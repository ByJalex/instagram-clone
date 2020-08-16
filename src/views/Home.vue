<template>
  <div class="home">
    <div class="header-home">
      <div class="header-home-son justify-between">
        <vs-avatar>
          <i class="bx bx-camera icons-header"></i>
        </vs-avatar>
        <vs-avatar badge badge-color="primary">
          <i class="bx bx-send icons-header"></i>
          <template #badge>10</template>
        </vs-avatar>
      </div>
    </div>
    <div class="break content-home">
      <div class="profileStories">
        <div class="content">
          <div style="margin-left: 10px" class="center con-avatars">
            <vs-avatar size="70" circle>
              <i class="bx bx-plus"></i>
            </vs-avatar>
            <div class style>
              <small class="userProfile">Me</small>
            </div>
          </div>
          <div class="icon-storie" v-for="index in 20" :key="index">
            <vs-avatar size="70" circle history history-gradient>
              <i class="bx bx-user"></i>
            </vs-avatar>
            <div class style>
              <small class="userProfile">Test</small>
            </div>
          </div>
        </div>
      </div>
      <div class="break-2"></div>
      <div class="content-photos" v-for="index in 10" :key="index">
        <div style="margin-top: 25px"></div>
        <div class="header-post">
          <vs-avatar>
            <i class="bx bx-user icons-header"></i>
          </vs-avatar>
          <div>josue_ayala27</div>
          <div>
            <i style="font-size: 25px" class="bx bx-dots-vertical-rounded"></i>
          </div>
        </div>
        <div class="content-post">
          <img
            class="responsive image-crop"
            src="https://images.unsplash.com/photo-1596888387677-ec9d3843424b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=750&q=80"
            alt
          />
        </div>
        <div class="icons-post justify-between">
          <div>
            <div>
              <i class='bx bx-heart bx-sm'></i>
              <i class='bx bx-comment bx-sm icon-left' ></i>
            </div>
          </div>
          <div>
            <i class='bx bx-collection bx-sm'></i>
          </div>
        </div>
        <div class="description-post">
          <b>josue_ayala27</b>
          <span>Fue un dia bastante grandioso, como me encantaria repetirlo.</span>
          <div class="likes">
            <small>
              Les gusta a
              <b>josue_test</b> y
              <b>7 personas más</b>.
            </small>
            <div class="content-group">
              <vs-avatar-group max="3">
                <vs-avatar v-for="index in 10" :key="index">
                  <i class="bx bx-user"></i>
                </vs-avatar>
              </vs-avatar-group>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="end">

    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
};
</script>

<style>

</style>
