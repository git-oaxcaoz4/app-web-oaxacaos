<template>
  <v-app>
    <v-content
      class="fill-height bg-no-repeat bg-cover align-center"
      :style="{ backgroundImage: `url(${backgroundUrl})` }"
    >
      <v-row justify="center">
        <v-col cols="12" sm="8" md="4">
          <v-card max-width="350" class="mx-auto">
            <v-img
              height="250"
              src="https://www.seekpng.com/png/detail/138-1388103_user-login-icon-login.png"
            ></v-img>
            <v-card-text>
              <v-form>
                <v-text-field
                  label="Login"
                  name="login"
                  prepend-icon="person"
                  type="text"
                />
                <v-text-field
                  id="password"
                  label="Password"
                  name="password"
                  prepend-icon="lock"
                  type="password"
                />
              </v-form>
            </v-card-text>
            <v-card-actions>
              <v-spacer />
              <v-btn color="primary">Iniciar sesión</v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-content>
  </v-app>
</template>

<script>
import backgroundUrl from "./assets/fondo3.jpg";
export default {
  data() {
    return {
      backgroundUrl,
      title: "Oaxacaos",
      menu: [{ name: "Iniciar sesión" }, { name: "Registrarse" }]
    };
  }
};
</script>
