<template>
    <div class="container is-max-desktop">

            <div class="box">
                <h1>PoveziME</h1>

            <router-link to="/vozac"><button class="button">VOZAČ</button></router-link>
            <router-link to="/putnik"><button class="button">PUTNIK</button></router-link>
            <router-link to="/paket"><button class="button">PAKET</button></router-link>
            <router-link to="/login"><button class="button">LOG IN</button></router-link>
            <router-link to="/about"><button class="button">HOME</button></router-link>
            </div>

            <div class="box2">
                
            <form>
            <b-field label="Ime">
             <b-input v-model="name"></b-input>
            </b-field>

            <b-field label="Email"
                type="is-danger"
                message="This email is invalid">
                <b-input type="email"
                 value="john@"
                 maxlength="30">
                </b-input>
            </b-field>

            <b-field label="Username"
             type="is-success"
             message="This username is available">
             <b-input value="johnsilver" maxlength="30"></b-input>
            </b-field>

            <b-field label="Password">
                <b-input type="password"
                    value="iwantmytreasure"
                    password-reveal>
                </b-input>
            </b-field>

            <b-field label="Poruka">
                <b-input maxlength="200" type="textarea"></b-input>
            </b-field>

            <button class="button">Obriši</button>
            <button class="button">Pošalji</button>
            </form>
            </div>
    </div>
</template>


<script>
    export default {
        data() {
            return {
                name: 'John Silver'
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.button {
    all: unset;
    font-familly: Roboto, sans-serif;
    font-size: 8pt;
    color: white;
    margin: 10px;
    padding: 10px;
    background-color: rgb(122, 113, 11, 0.7);
    border-radius: 15px 0px;
    width: 10%;
}

.button:hover {
    background-color:#ffffff;
    color: rgb(122, 113, 11, 0.7);
}

.box, .box2{
    background-color: rgba(24, 22, 22, 0.4);
    padding: 40px;
    font-size: 50px;
    border-radius: 4px;
    margin: 10px;
    color: white;
}

a {text-decoration: none;}
.is-primary {background-color: white;}
router-link {text-decroation: none;}

label {
    color: white;
}

</style>
