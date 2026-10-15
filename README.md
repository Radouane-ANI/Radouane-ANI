<div align="center">

# 👋 Radouane Aouini

### 🎓 Étudiant en Master Cryptologie, Calcul de Haute Performance et Algorithmie (CCA)
**Sorbonne Université / Université Paris Cité**

*Cryptanalyse & Sécurité Logicielle • Calcul Haute Performance (MPI / OpenMP / CUDA) • Arithmétique Mixte • Algorithmique Avancée & Complexité*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Radouane%20AOUINI-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/radouane-aouini-b14bab348)
[![GitHub](https://img.shields.io/badge/GitHub-Radouane--ANI-181717?style=for-the-badge&logo=github)](https://github.com/Radouane-ANI)
[![Email](https://img.shields.io/badge/Contact-Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:radouane.aouini@outlook.com)

---

### 💻 Technologies & Environnement Technique

![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![MPI](https://img.shields.io/badge/MPI-Parallel-blue?style=flat-square)
![OpenMP](https://img.shields.io/badge/OpenMP-Multithreaded-orange?style=flat-square)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![OCaml](https://img.shields.io/badge/OCaml-EC6813?style=flat-square&logo=ocaml&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-e16737?style=flat-square&logo=mathworks&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![x86_64 ASM](https://img.shields.io/badge/x86__64_ASM-000000?style=flat-square&logo=assemblyscript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Linux HPC](https://img.shields.io/badge/Linux_HPC-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## 🎯 Projets Phares & Recherche Académique

<table>
  <!-- Section 1 : Cryptographie & HPC -->
  <tr>
    <td colspan="2" bgcolor="#1f242c">
      <h3 style="margin: 0; color: #58a6ff;">🛡️ Cryptographie & Calcul Haute Performance (HPC)</h3>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/Radouane-ANI/Meet-in-the-Middle">🚀 Meet-in-the-Middle (SPECK-64/128)</a></h4>
      <p><b>Attaque cryptanalytique distribuée massive sur supercalculateur Grid5000</b></p>
      <ul>
        <li>Recherche de collisions <i>golden claw</i> sur le chiffrement par bloc SPECK-64/128 (NSA).</li>
        <li><b>Architecture Hybride MPI + OpenMP</b> (<code>MPI_THREAD_MULTIPLE</code>, sharding déterministe de la mémoire du dictionnaire).</li>
        <li>Gestion fine de la contention avec <b>65 536 verrous <code>omp_lock_t</code></b> et pipeline asynchrone producteur-consommateur avec <code>#pragma omp task</code>.</li>
        <li><b>Résultat Grid5000 :</b> Passage de <b>1 637 s (27 min) à 25,3 s</b>, soit une <b>accélération spectaculaire de ×65</b> face à la version séquentielle.</li>
      </ul>
      <p><i>Technologies : C99, MPI, OpenMP, Cluster Grid5000</i></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/Radouane-ANI/auctionp2p">🌐 AuctionP2P (Protocole Pair-à-Pair IPv6)</a></h4>
      <p><b>Application distribuée d'enchères sécurisées en réseau décentralisé</b></p>
      <ul>
        <li>Architecture P2P résiliente en IPv6 natif avec découverte multicast et échanges TCP/UDP.</li>
        <li>Sécurisation cryptographique intégrale des offres et des transactions par <b>signatures asymétriques ED25519</b>.</li>
        <li>Protocole de consensus distribué entre pairs pour l'attribution transparente et horodatée des enchères.</li>
      </ul>
      <p><i>Technologies : C, IPv6, Cryptographie ED25519, Systèmes Distribués</i></p>
    </td>
  </tr>

  <!-- Section 2 : Calcul Numérique & Précision Mixte -->
  <tr>
    <td colspan="2" bgcolor="#1f242c">
      <h3 style="margin: 0; color: #58a6ff;">⚡ Algèbre Linéaire Numérique, HPC & Précision Mixte</h3>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/Radouane-ANI/Projet-cca">📊 GEP Mixte : Factorisation ILU en Précision Mixte</a></h4>
      <p><b>Préconditionnement adaptatif pour solveurs linéaires GMRES (Sous la direction de Théo Mary, LIP6)</b></p>
      <ul>
        <li>Conception d'un préconditionneur ILUT creux à allocation dynamique de précision (FP16, FP24, FP32, FP48, FP64) élément par élément.</li>
        <li>Critère d'affectation fondé sur la norme de colonne garantissant que l'erreur d'arrondi numérique ne dépasse pas la tolérance de chute $\varepsilon$.</li>
        <li>Évaluation sur la collection de matrices <b>SuiteSparse</b> (réseaux électriques, réservoirs pétroliers, aérospatiale) : <b>compression mémoire jusqu'à 3.8×</b> avec 100% de convergence et profils de Dolan-Moré optimaux.</li>
      </ul>
      <p><i>Technologies : MATLAB, Précision Mixte (chop), GMRES, LaTeX</i></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/Radouane-ANI/Polynomial-Multiplication">🔢 Polynomial Multiplication & Stabilité MPFR</a></h4>
      <p><b>Algorithmes rapides de multiplication polynomiale et analyse numérique</b></p>
      <ul>
        <li>Implémentation comparative multi-algorithmes : Naïf $\mathcal{O}(n^2)$, Karatsuba $\mathcal{O}(n^{\log_2 3})$, Toom-Cook-3 et Toom-4.</li>
        <li>Étude rigoureuse de la stabilité numérique et des propagations d'erreurs en virgule flottante en utilisant la bibliothèque multiprécision arbitraire <b>GNU MPFR</b> comme référence exacte.</li>
      </ul>
      <p><i>Technologies : C, GNU MPFR, Optimisation Algorithmique</i></p>
    </td>
  </tr>

  <!-- Section 3 : Algorithmie & Logique -->
  <tr>
    <td colspan="2" bgcolor="#1f242c">
      <h3 style="margin: 0; color: #58a6ff;">📐 Algorithmique Avancée, Complexité & Méthodes Formelles</h3>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/Radouane-ANI/Optimisation-Vertex-Cover">🎯 Optimisation du Vertex Cover (Couverture par Sommets)</a></h4>
      <p><b>Algorithmes exacts et heuristiques pour un problème NP-difficile</b></p>
      <ul>
        <li>Algorithmes exacts : Branch & Bound classique et Branch & Bound hautement optimisé par élagage via bornes inférieures de couplage maximal.</li>
        <li>Algorithmes approchés : Glouton par degré maximal et 2-approximation par couplage maximal.</li>
        <li>Banc d'essai et benchmarks expérimentaux sur graphes aléatoires d'Erdős-Rényi $G(n, p)$ avec visualisations Matplotlib.</li>
      </ul>
      <p><i>Technologies : Python, Théorie des Graphes, NP-Hard, Matplotlib</i></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/Radouane-ANI/DPLL-SAT-Solver-ocaml">🧩 Solveur DPLL SAT en OCaml</a></h4>
      <p><b>Moteur de résolution de satisfiabilité booléenne en programmation fonctionnelle</b></p>
      <ul>
        <li>Implémentation rigoureuse de l'algorithme Davis-Putnam-Logemann-Loveland (DPLL) sur instances au standard DIMACS.</li>
        <li>Heuristiques d'optimisation : propagation unitaire, élimination des littéraux purs et choix dynamique de branchement.</li>
      </ul>
      <p><i>Technologies : OCaml, Méthodes Formelles, Logique Propositionnelle</i></p>
    </td>
  </tr>

  <!-- Section 4 : Systèmes Bas-Niveau, Compilateurs & Systèmes Multi-Agents -->
  <tr>
    <td colspan="2" bgcolor="#1f242c">
      <h3 style="margin: 0; color: #58a6ff;">⚙️ Systèmes d'Exploitation, Compilateurs & Systèmes Multi-Agents</h3>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/Radouane-ANI/fsh-c">🐚 fsh-c (Shell Unix en C)</a></h4>
      <p>Interpréteur de commandes Unix avec redirections <code>&lt;</code>, <code>&gt;</code>, <code>&gt;&gt;</code>, pipelines <code>|</code>, gestion de signaux POSIX et boucles de contrôle <code>for</code>.</p>
      <h4><a href="https://github.com/Radouane-ANI/compilateur-simpletxt">📝 Compilateur SimpleText vers HTML</a></h4>
      <p>Chaîne de compilation complète en OCaml (Lexer <code>ocamllex</code>, Parser <code>Menhir</code>, AST) avec table de macros dynamiques et génération HTML.</p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/Radouane-ANI/dedale">🗺️ Dedale (Systèmes Multi-Agents JADE)</a></h4>
      <p>Plateforme distribuée sous JADE pour l'exploration coopérative décentralisée et la traque coordonnée de créatures mobiles en environnement partiellement observable.</p>
      <h4><a href="https://github.com/Radouane-ANI/big-match">💘 Big Match (Base de Données Relationnelle SQL)</a></h4>
      <p>Modélisation relationnelle complète (E/A, 3NF), contraintes d'intégrité et requêtes analytiques avancées pour une application de rencontres culturelles.</p>
    </td>
  </tr>
</table>

---

### 📈 Statistiques GitHub

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Radouane-ANI&show_icons=true&theme=radical&hide_border=true&count_private=true" alt="Statistiques GitHub" height="160"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Radouane-ANI&layout=compact&theme=radical&hide_border=true" alt="Langages les plus utilisés" height="160"/>
</div>
