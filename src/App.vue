<template>
  <div id="content">
    <b-navbar toggleable="lg" type="dark" variant="dark">
      <div class="container col-11">
        <b-navbar-brand href="#">Piersanti Dylan</b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item active right>Accueil</b-nav-item>
            <b-nav-item right>Compétences</b-nav-item>
            <b-nav-item right>Portfolio</b-nav-item>
            <b-nav-item right>Expérience</b-nav-item>
            <b-nav-item right>Contact</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </div>
    </b-navbar>

    <header class="row">
      <b-card
        no-body
        class="overflow-hidden col-lg-11 col-md-10.5 col-xs-10.5 mx-5"
        style="max-width: 100%; color: #fff"
        bg-variant="dark"
      >
        <b-row no-gutters>
          <b-col md="6">
            <b-card-img :src="profil" class="rounded-0" style="padding: 15px 0 15px 0"></b-card-img>
            <ul class="socialList">
              <li>
                <a href="#" class="fab fa-facebook-messenger"></a>
              </li>
              <li>
                <a href="#" class="fab fa-twitter"></a>
              </li>
              <li>
                <a href="#" class="fab fa-github"></a>
              </li>
              <li>
                <a href="#" class="fab fa-linkedin"></a>
              </li>
              <li>
                <a href="#" class="fa fa-comment"></a>
              </li>
            </ul>
          </b-col>
          <b-col md="6">
            <b-card-body title="Piersanti dylan">
              <b-card-text>
                <h6>Graphiste & Développeur web</h6>
                <b-button variant="success" class="myButtons">Download CV</b-button>
                <b-button variant="primary" class="myButtons">Me contacter</b-button>
                <div class="row">
                  <ul class="col-12">
                    <li>
                      <h4 class="fa fa-birthday-cake">- 17/08/1994</h4>
                    </li>
                    <li>
                      <h4 class="fa fa-home">- 55120 - Auzeville</h4>
                    </li>
                    <li>
                      <h4 class="fa fa-phone">- 07.68.45.52.69</h4>
                    </li>
                  </ul>
                </div>
              </b-card-text>
            </b-card-body>
          </b-col>
        </b-row>
      </b-card>
      <b-container class="bv-example-row">
        <b-row class="blockContent">
          <b-col class="competences mx-5">Column</b-col>
          <b-col class="experience mx-5">Column</b-col>
        </b-row>
      </b-container>
    </header>

    <div class="blockContent row col-12"></div>
  </div>
</template>

<script>
import profil from "./assets/profilPhoto.png";

export default {
  name: "app",
  data() {
    return {
      profil
    };
  }
};
</script>

<style>

header {
  position: absolute;
  left: 25%;
  margin-top: 220px;
  max-width: 1366px;
  text-align: center;
}

.infos {
  margin-left: 50px;
}

.myButtons {
  margin: 0 15px 0 0;
}

li {
  margin-top: 40px;
  margin-left: 30px;
  list-style: none;
  font-size: 13px;
  text-align: left;
}

.socialList li {
  display: inline;
  margin: 0 0 0 25px;
}

.socialList {
  margin-left: -50px;
}

.socialList li a {
  font-size: 25px;
  color: #fff;
  text-decoration: none;
}

.middContainer {
  background-color: #fff;
  height: 500px;
  width: 200px;
}

.blockContent {
  margin-top: 25px;
}

.competences, .experience {
  height: 200px;
  width: 300px;
  background-color: #272c2e;
}
@media (max-width: 1367px) {
  header {
    position: absolute;
    right: 5%;
    left: 7%;
    width: 90%;
    margin-top: 80px;
  }

  li {
    margin-top: 40px;
    list-style: none;
    font-size: 13px;
    text-align: center;
  }

  .socialList {
    margin-left: 15%;
  }

  @media (max-width: 900px) {
    .socialList {
      margin-left: -8px;
    }
  }
}
</style>
