---
layout: null
---
<style>
  body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; line-height: 1.6; color: #333; max-width: 1000px; margin: 0 auto; padding: 20px; background-color: #f9f9f9; }
  h1, h2, h3 { color: #111; text-align: center; }
  .section-title { font-size: 2em; margin-bottom: 5px; margin-top: 40px;}
  .section-line { width: 50px; height: 3px; background-color: #007bff; margin: 0 auto 30px auto; }
  
  /* Section Profil */
  .profile-container { display: flex; gap: 40px; background: white; padding: 40px; border-radius: 12px; box-shadow: 0 4px 6px rgba(0,0,0,0.05); margin-bottom: 50px; align-items: center; }
  
  /* --- CORRECTION DE L'IMAGE DE PROFIL (CERCLE PARFAIT ET PAS DE BANDES NOIRES) --- */
  .profile-image {
    flex: 0 0 200px; /* Non-flexible, largeur fixe de 200px */
    width: 200px;
    height: 200px;
    overflow: hidden; /* Masque tout ce qui dépasse du cercle */
    border-radius: 50%; /* Cercle parfait */
    box-shadow: 0 4px 8px rgba(0,0,0,0.1); /* Ombre douce */
    border: 4px solid #fff; /* Anneau blanc élégant */
    display: flex; /* Centrage de l'image si elle est petite */
    justify-content: center;
    align-items: center;
  }
  .profile-image img {
    width: 100%;
    height: 100%;
    object-fit: cover; 
    object-position: center 15%; /* Magie : indique au site de viser le "haut" de l'image là où se trouve le visage */
  }
  /* --------------------------------------------------------------------------------- */

  .profile-text { flex: 2; }
  .profile-title { font-size: 1.5em; color: #007bff; font-weight: bold; margin-bottom: 5px; margin-top: 0;}
  .profile-subtitle { color: #666; font-weight: bold; margin-bottom: 20px; font-size: 1.1em; }
  .tech-stack { color: #666; font-size: 0.9em; margin-top: 20px; padding-top: 15px; border-top: 1px dashed #eee; }
  
  /* Section Projets (Cartes) */
  .projects-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(350px, 1fr)); gap: 30px; margin-bottom: 50px; }
  .project-card { background: white; padding: 30px; border-radius: 12px; box-shadow: 0 4px 6px rgba(0,0,0,0.05); border: 1px solid #eee; display: flex; flex-direction: column; }
  .project-title { color: #007bff; font-size: 1.4em; margin-top: 0; margin-bottom: 15px; text-align: left;}
  .project-desc { flex-grow: 1; margin-bottom: 20px; color: #555; }
  .project-tools { color: #888; font-size: 0.85em; margin-top: 20px; border-top: 1px dashed #eee; padding-top: 15px; }
  
  /* Section Background (Timeline) */
  .background-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 40px; margin-bottom: 50px; }
  .timeline-col h3 { text-align: left; color: #111; margin-bottom: 30px; font-size: 1.5em;}
  .timeline-item { border-left: 3px solid #007bff; padding-left: 20px; margin-bottom: 30px; position: relative; }
  .timeline-item::before { content: ''; position: absolute; left: -9px; top: 0; width: 15px; height: 15px; background: white; border: 3px solid #007bff; border-radius: 50%; }
  .timeline-date { color: #888; font-size: 0.9em; margin-bottom: 5px; font-weight: bold;}
  .timeline-title { font-weight: bold; color: #333; font-size: 1.1em; margin-bottom: 2px;}
  .timeline-subtitle { color: #555; font-style: italic; margin-bottom: 10px; font-size: 0.95em;}
  .timeline-desc { color: #555; font-size: 0.95em; margin-bottom: 5px;}
  .timeline-tools { font-size: 0.85em; color: #888; margin-top: 5px; font-style: italic;}

  /* Boutons */
  .btn-group { display: flex; gap: 15px; margin-bottom: 10px; }
  .btn { display: inline-block; padding: 8px 20px; border: 2px solid #007bff; color: #007bff; text-decoration: none; border-radius: 6px; font-weight: 600; font-size: 0.9em; transition: all 0.2s; }
  .btn:hover { background-color: #007bff; color: white; }
  .btn-solid { background-color: #2563eb; color: white; border: none; padding: 12px 25px; border-radius: 8px; font-size: 1em; text-decoration: none; font-weight: bold;}
  .btn-solid:hover { background-color: #1d4ed8; color: white; text-decoration: none;}
  
  /* Section Contact */
  .contact-section { text-align: center; margin-top: 60px; padding: 40px 0; }
  .contact-buttons { display: flex; justify-content: center; gap: 20px; margin-top: 20px; }
  
  @media (max-width: 768px) {
    .profile-container { flex-direction: column; text-align: center; }
    .projects-grid, .background-grid { grid-template-columns: 1fr; }
    .timeline-col h3 { text-align: center; }
  }
</style>

<h1 class="section-title">Profil Professionel</h1>
<div class="section-line"></div>

<div class="profile-container">
  <div class="profile-image">
    <img src="images/photo.jpg" alt="Minan Jean-Marc Ouattara" onerror="this.style.display='none'">
  </div>
  <div class="profile-text">
    <p class="profile-title">Minan Jean-Marc OUATTARA</p>
    <p class="profile-subtitle">Data analyst</p>
    <p>Je suis un data analyst doté d'une solide formation en économétrie et en analyse économique.</p>
    <p>Je conçois des solutions analytiques de bout en bout pour extraire de la valeur des données allant de la construction de pipelines de nettoyage (ETL) et de l'analyse exploratoire (EDA), jusqu'à la modélisation prédictive (Machine Learning). J'applique ces méthodes à des problématiques variées, telles que l'analyse de marché, l'intelligence client (e-commerce) et l'évaluation de performances.</p>
    <p>Au-delà de l'analyse statistique, j'attache une grande importance à l'industrialisation et à la restitution de mes travaux. Je développe des applications interactives (Streamlit), crée des API REST (FastAPI) pour l'intégration des modèles, et assure la reproductibilité de mes environnements (Docker, Poetry).</p>
    <p><strong> Actuellement en Master 2 Statistiques pour l'Évaluation et la Prévison, je recherche un stage de fin d’études pour contribuer à la valorisation de vos données et soutenir vos décisions stratégiques.</strong></p>
    <div class="tech-stack"><strong>Stack Technique :</strong> Python (Pandas, Scikit-Learn, FastAPI, Streamlit), SQL, Power BI, R, Excel (VBA), Docker.</div>
  </div>
</div>

<h2 class="section-title">Projets</h2>
<div class="section-line"></div>
<p style="text-align: center; margin-bottom: 40px; color: #666;">Voici une sélection de mes projets en analyse de données, modélisation et développement d'applications.</p>

<div class="projects-grid">
  
  <div class="project-card">
    <h3 class="project-title">NFL Offense Analytics (2005-2024)</h3>
    <div class="project-desc">
      <strong>Pipeline de données complète (End-to-End) sur des données sportives web-scrapées.</strong><br><br>
      Missions : Nettoyage (ETL), feature engineering, analyse exploratoire (EDA) et modélisation prédictive (Random Forest) des performances offensives. Intégration d'un dashboard interactif et d'une API.
    </div>
    <div class="btn-group">
      <a href="https://github.com/ouat225/the-redzone-predictor" class="btn" target="_blank">GitHub Repo</a>
    </div>
    <div class="project-tools">Outils : Python, Scikit-Learn, Streamlit, FastAPI, Pytest.</div>
  </div>

  <div class="project-card">
    <h3 class="project-title">MaisonEstimateur</h3>
    <div class="project-desc">
      <strong>Outil interactif d'analyse du marché immobilier basé sur 10 000 logements.</strong><br><br>
      Missions : Réalisation d'analyses statistiques univariées et multivariées. Développement d'une application de visualisation. Gestion rigoureuse de l'environnement avec Poetry et intégration de tests unitaires.
    </div>
    <div class="btn-group">
      <a href="https://github.com/ouat225/management-de-projets-digitaux" class="btn" target="_blank">GitHub Repo</a>
    </div>
    <div class="project-tools">Outils : Python, Streamlit, Poetry, Pytest, Pandas.</div>
  </div>

  <div class="project-card">
    <h3 class="project-title">Écosystème Wyverne</h3>
    <div class="project-desc">
      <strong>Simulation interactive de dynamique de populations.</strong><br><br>
      Missions : Modélisation mathématique (taux de croissance/compétition). Création d'une API REST pour exposer les données et d'un tableau de bord, le tout entièrement conteneurisé.
    </div>
    <div class="btn-group">
      <a href="https://github.com/ouat225/ecosysteme-des-donnees" class="btn" target="_blank">GitHub Repo</a>
    </div>
    <div class="project-tools">Outils : Python, Docker, FastAPI, Streamlit, NumPy.</div>
  </div>

</div>

<h2 class="section-title">Mon Parcours</h2>
<div class="section-line"></div>

<div class="background-grid">
  
  <div class="timeline-col">
    <h3>Études</h3>
    
    <div class="timeline-item">
      <div class="timeline-date">2024 - 2026</div>
      <div class="timeline-title">Master 2 Statistiques pour l'Évaluation et la Prévision</div>
      <div class="timeline-subtitle">Université de Reims Champagne-Ardenne</div>
    </div>
    
    <div class="timeline-item">
      <div class="timeline-date">2021 - 2024</div>
      <div class="timeline-title">Licence Économie et Gestion, parcours Analyse Économique</div>
      <div class="timeline-subtitle">Université de Reims Champagne-Ardenne</div>
    </div>
  </div>

  <div class="timeline-col">
    <h3>Expériences Professionnelles</h3>
    
    <div class="timeline-item">
      <div class="timeline-date">01/2024 - 03/2024</div>
      <div class="timeline-title">Analyste de Marché (Stage)</div>
      <div class="timeline-subtitle">ISLT, Troyes</div>
      <div class="timeline-desc">• Collecte et interprétation de données clients pour évaluer la demande concurrentielle.</div>
      <div class="timeline-desc">• Utilisation de R et Python pour l'analyse descriptive et la visualisation.</div>
      <div class="timeline-tools">Outils : R, Python, Excel</div>
    </div>
    
    <div class="timeline-item">
      <div class="timeline-date">06/2022 - 09/2022</div>
      <div class="timeline-title">Stagiaire E-commerce Analyste</div>
      <div class="timeline-subtitle">DASH, Abidjan</div>
      <div class="timeline-desc">• Analyse des ventes et des comportements clients pour identifier les leviers de croissance.</div>
      <div class="timeline-desc">• Suivi des KPI et analyse des performances pour la stratégie marketing digitale.</div>
      <div class="timeline-tools">Outils : Excel, SQL</div>
    </div>
    
    <div class="timeline-item">
      <div class="timeline-date">06/2020 - 08/2020</div>
      <div class="timeline-title">Stagiaire Comptabilité</div>
      <div class="timeline-subtitle">Ambassade de Côte d'Ivoire, Addis-Abeba</div>
      <div class="timeline-desc">• Numérisation, vérification des données comptables et préparation de rapports.</div>
      <div class="timeline-tools">Outils : Excel</div>
  </div>

</div>

<div class="contact-section">
  <h2 class="section-title">Let's Connect</h2>
  <div class="section-line"></div>
  <p>Vous êtes intéressé par mon profil ou souhaitez discuter d'un projet ? N'hésitez pas à me contacter.</p>
  
  <div class="contact-buttons">
    <a href="mailto:ouattaramjeanmarc@gmail.com" class="btn-solid">Email</a>
    <a href="https://www.linkedin.com/in/minan-jean-marc-ouattara-809061291/" class="btn-solid" target="_blank">LinkedIn</a>
    <a href="https://github.com/ouat225" class="btn-solid" target="_blank">GitHub</a>
  </div>
</div>
