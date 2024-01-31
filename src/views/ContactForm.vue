<template>
    <div class="contact-form-container">
        <form @submit.prevent="submitForm">
            <h1>Kontakta mig</h1>
            <input type="text" v-model="form.name" placeholder="Ditt namn" required>
            <input type="email" v-model="form.email" placeholder="Din e-post" required>
            <textarea v-model="form.message" placeholder="Ditt meddelande" required></textarea>
            <button type="submit" class="submit-btn">Skicka Meddelande</button>
        </form>
    </div>
</template>

<script>
export default {
    name: 'ContactForm',
    data() {
        return {
            form: {
                name: '',
                email: '',
                message: ''
            }
        }
    },
    methods: {
        submitForm() {
            // Här skulle du hantera inskick av formuläret, t.ex. göra en API-anrop
            console.log(this.form);
            alert("Meddelande skickat!");
            // Efter inskick kan du rensa formuläret
            this.form.name = '';
            this.form.email = '';
            this.form.message = '';
        }
    }
}
</script>

<style scoped>
.contact-form-container {
    background-color: #f1c6b8;
    padding: 30px;
    margin-top: 4rem;
    border-radius: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

form {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

input[type="text"],
input[type="email"],
textarea {
    border: none;
    padding: 15px;
    border-radius: 15px;
    margin-bottom: 10px;
}

textarea {
    height: 100px;
    resize: none;
}

.submit-btn {
    background-color: white;
    color: black;
    padding: 15px 20px;
    border: none;
    border-radius: 20px;
    cursor: pointer;
    font-size: 16px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
    transition: background-color 0.3s ease;
}
.submit-btn{
  border: 0 solid;
  box-shadow: inset 0 0 20px rgba(255, 255, 255, 0);
  outline: 1px solid;
  outline-color: rgba(255, 255, 255, .5);
  outline-offset: 0px;
  text-shadow: none;
  transition: all 1250ms cubic-bezier(0.19, 1, 0.22, 1);
} 

.submit-btn:hover {
  border: 1px solid;
  box-shadow: inset 0 0 20px rgba(255, 255, 255, .5), 0 0 20px rgba(255, 255, 255, .2);
  outline-color: rgba(255, 255, 255, 0);
  outline-offset: 15px;
  text-shadow: 1px 1px 2px #f1c6b8; 
}

.submit-btn:hover {
    transform: translate(0,-1px);
}

.submit-btn::after {
    content: '→';
    display: block;
    margin-left: 10px;
}

@media (max-width: 600px) {
    .contact-form-container {
        width: 100%;
        box-sizing: border-box;
        margin: 10px;
    }
}
</style>
