<template>
  <Section class="profile">
    <img src="../assets/1516370067758.jpeg" />
    <TextSection>
      <h2>Qui suis-je?</h2>
      <p class="bold">François VIENNOT</p>
      <p>
        Ex-directeur de projet ferroviaire, animé par le désir d’entreprendre et
        de transmettre, propose des prestations ponctuelles au service de vos
        projets.
      </p>
    </TextSection>
  </Section>
</template>

<style lang="scss" scoped>
div.profile {
  div.bloc {
    background-color: var(--vt-c-orange);
    max-width: 600px;
  }
  background-color: var(--vt-c-orange);
  color: white;
  align-items: center;
  justify-content: center;

  img {
    padding: 10px;
    border-radius: 50%;
    border: 4px solid whitesmoke;
    height: 200px;
  }

  p {
    font-size: 1.3em;
    span.bold {
      font-weight: bold;
    }
  }
}

@media screen and (max-width: 900px) {
  div.profile {
    display: flex;
    flex-flow: column;
  }
}
</style>