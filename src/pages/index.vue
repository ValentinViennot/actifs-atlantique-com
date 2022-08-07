<template>
  <div id="body">
    <SeaSkyAnimation>
      <div id="header">
        <h1>ACTIFS Atlantique</h1>
        <div>
          <span>Activités</span>
          <span>Formations</span>
          <span>Séminaires</span>
        </div>
      </div>
    </SeaSkyAnimation>
    <TextSection id="home_text">
      <p>
        La côte de Jade en Loire Atlantique présente tous les atouts d’un cadre
        exceptionnel propice à votre séminaire thématique.
      </p>
      <p>
        ACTIFS Atlantique vous accompagne dans la préparation et l’organisation
        de cet évènement qui répondra à votre attente pour la plus grande
        satisfaction de vos collaborateurs.
      </p>
      <p class="bold">
        La garantie d’un évènement sur mesure en cohérence avec vos
        objectifs&nbsp;!
      </p>
    </TextSection>
    <Quote>Un espace à découvrir</Quote>
    <Squares>
      <Square
        title="Activités"
        description="éloignées du quotidien pour améliorer la cohésion du groupe"
      />
      <Square
        title="Convivialité"
        description="permettant de favoriser le dialogue et les échanges"
      />
      <Square
        title="Tourisme"
        description="découverte d'environnements différents du quotidien…"
      />
      <Square
        title="Industriel"
        description="sur un thème prédéfini ensemble"
      />
      <Square
        title="Formation"
        description="spécifique pour répondre au besoin identifié"
      />
      <Square
        title="Séminaire"
        description="thématique, en accord avec vos objectifs…"
      />
    </Squares>
    <Section id="logo">
      <img src="../assets/logo.png" />
      <TextSection>
        <h2>Qu'est-ce que ACTIFS Atlantique?</h2>
        <p>
          ACTIFS pour vos projets : la dynamique d’un réseau mise à votre
          service pour vous accompagner lors d’évènements d’entreprises tels que
          séminaires, conférences, découvertes d’autres environnements :
          tourisme industriel, ou encore des activités extra professionnelles
          (ludiques, originales, sportives…) afin de renforcer l’esprit d’équipe
          au service de vos projets.
        </p>
      </TextSection>
    </Section>
    <Quote>Expertise Métier Passion</Quote>
    <TextSection id="backorange">
      <h2>Pourquoi choisir ACTIFS Atlantique ?</h2>
      <p class="bold">
        ACTIFS dans vos projets, une dynamique soutenue par des actions ciblées
        déterminées par une analyse systémique construite sur l’expérience des
        grands projets et la connaissance du système ferroviaire.
      </p>
    </TextSection>
    <Squares id="values">
      <Square title="Analyse" />
      <Square title="Conseil" />
      <Square title="Technique" />
      <Square title="Ingénierie" />
      <Square title="Ferroviaire" />
      <Square title="Systèmes" />
    </Squares>
    <Profile />
    <ContactForm />
    <Footer />
  </div>
</template>

<style lang="scss" >
div#body {
  background-image: url("../assets/st_michel.png");
  // background-image: url("../assets/st_michel_pixels.png");
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  div#backorange {
    background-color: var(--vt-c-indigo);
    color: white;
  }

  div#values {
    width: 100%;
    > div.squares_bloc {
      width: 600px;
    }
  }

  div#header {
    width: 100%;
    top: 30%;
    z-index: 10;
    text-align: center;
    display: block;
    color: #4c545e;
    font-family: "Josefin";
    text-transform: uppercase;
    > h1 {
      font-size: 6em;
    }
    > div > span {
      font-size: 2em;
      padding-right: 0.5em;
      padding-left: 0.5em;
    }
  }
}

@media screen and (max-width: 900px) {
  div#body {
    div#logo {
      img {
        display: none;
      }
      div {
        padding: 0;
      }
    }

    div#header {
      > h1 {
        font-size: 3em;
      }
      > div {
        > span {
          display: block;
          padding-top: 0.5em;
          font-size: 1.5em;
        }
      }
    }
  }
}

@media screen and (max-width: 1270px) {
  div.squares_bloc {
    max-width: 600px;
  }
}
</style>
