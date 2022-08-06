<template>
  <TextSection>
    <h2>Me contacter</h2>
    <form
      action="https://formspree.io/f/mzbwpqrb"
      method="POST"
      enctype="multipart/form-data"
    >
      <form action="https://formspree.io/f/mzbwpqrb" method="POST">
        <label>
          Votre email:
          <input type="email" name="email" placeholder="hello@example.com" />
        </label>
        <label>
          Votre message:
          <textarea name="message"></textarea>
        </label>
        <!-- your other form fields go here -->
        <button type="submit">Envoyer</button>
      </form>
    </form>
  </TextSection>
</template>

<style lang="scss" scoped>
div.bloc {
  background-color: #f2f2f2;
}

form {
  width: 100%;
  display: flex;
  flex-flow: column;
  text-align: center;
  justify-content: center;

  label {
    width: 100%;
    margin: 10px 0;
    display: flex;
    flex-flow: column;
    text-align: left;

    input {
      padding: 10px;
    }

    textarea {
      min-height: 70px;
    }
  }

  button {
    margin: 20px 0;
    padding: 10px;
    background-color: var(--vt-c-indigo);
    border: none;
    color: white;
    border-radius: 5px;
  }
}
</style>
