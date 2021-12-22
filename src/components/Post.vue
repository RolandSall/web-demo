<template>
  <v-card class="my-3" elevation="1">
    <v-container class="py-4 px-10">
      <v-layout justify-space-around row wrap style="place-items: center">
        <div>
          <div class="post-title">
            Item Title
          </div>
          <v-icon
              class="icon"
              right
              size=8
          >
            lens
          </v-icon>
          <div class="user"> User Name</div>
        </div>
        <div style="flex-grow: 1; text-align: end">Nov 13, 2022</div>
      </v-layout>
      <v-layout justify-space-between row wrap>
        <v-flex lg4 md4 xs12>
          <h1 style="font-size: medium; padding-top: 15px">Section 1</h1>
          <div class="post-data"> Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum
            has been the
            industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and
            scrambled it to make a type specimen book. It has survived not only five centuries.
          </div>
        </v-flex>
        <v-flex lg4 md4 xs12>
          <h1 style="font-size: medium; padding-top: 15px">Section 2</h1>
          <div class="post-data"> Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum
            has been the
            industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and
            scrambled it to make a type specimen book. It has survived not only five centuries.
          </div>
        </v-flex>
        <v-flex lg2 md2 style="display: flex; place-items: end;" xs12>
          <div style="flex-grow: 1">
            <div class="checkout-data d-flex" style="place-items: center">
              <v-img
                  :src="require('../assets/icon.png')"
                  contain
                  height="35"
              ></v-img>
              <div class="text-h1 align-center" style="text-align: center; flex-grow: 1">
                2000 USD
              </div>
            </div>
            <SubmitButton/>
          </div>

        </v-flex>

      </v-layout>
      <div style="margin-top: 5px; font-weight: bold; color: black">Due June 1, 2022</div>

    </v-container>
  </v-card>
</template>


<script>
import SubmitButton from "./Buttons/SubmitButton";

export default {
  components: {SubmitButton}
}
</script>
<style>
.post-title {
  font-family: 'Times New Roman';
  font-weight: bold;
  color: #66032c;
  font-size: 25px;
  display: inline;
}

.user {
  font-family: 'Times New Roman';
  font-weight: bold;
  color: #8e8287;
  font-size: 17px;
  display: inline;
}

.icon {
  line-height: 2.5;
}

.post-date {
  font-family: 'Times New Roman';
  font-weight: bold;
  color: #8e8287;
  font-size: 20px;
  display: inline;
}

.post-data {
  font-family: 'Times New Roman';
  color: #000000;
  text-align: justify;
  text-justify: inter-word;

}

.checkout-data {
  font-family: 'Times New Roman';
  font-weight: bold;
  font-size: 20px;
  color: #66032c;


}

</style>
