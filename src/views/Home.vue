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
            <vs-avatar size="70">
              <i class="bx bx-plus"></i>
            </vs-avatar>
            <div class style>
              <small class="userProfile">Me</small>
            </div>
          </div>
          <div class="icon-storie" v-for="index in 20" :key="index">
            <vs-avatar size="70">
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
.justify-between {
  display: flex;
  justify-content: space-between;
}

.icons-header {
  font-size: 30px;
}

.header-home {
  overflow: hidden;
  background-color: white;
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 100;
  box-shadow: 0 1px 40px -20px rgba(0, 0, 0, 0.75);
}

.break {
  margin-top: 70px;
}

.break-2 {
  margin-top: 20px;
}
.header-home-son {
  padding: 10px;
}
.content-home {
  margin-left: 10px;
  margin-right: 10px;
}

.stories {
  background-color: red;
}

.profileStories::-webkit-scrollbar {
  display: none;
}
.profileStories {
  overflow-x: scroll;
  width: 100%;
}

.content {
  text-align: center;
  display: inline-flex;
  text-align: center;
  margin-top: 10px;
}

.icon-storie {
  margin-left: 10px;
}

.content-photos {
  /*a*/
}

.header-post {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.content-post {
  margin-top: 20px;
  margin-left: 10px;
  margin-right: 10px;
}

.description-post {
  margin-top: 20px;
  margin-left: 10px;
  margin-right: 10px;
}

.icons-post{
  margin-top: 20px;
  margin-left: 10px;
  margin-right: 10px;
}

.image-crop {
  border-radius: 30px 30px 30px 30px;
  -moz-border-radius: 30px 30px 30px 30px;
  -webkit-border-radius: 30px 30px 30px 30px;
  border: 0px solid #000000;
  box-shadow: 0 25px 40px -20px rgba(0, 0, 0, 0.75);
}

.icon-left{
  margin-left: 10px;
}

.responsive {
  max-width: 100%;
  height: auto;
}

.likes {
  margin-top: 10px;
}

.content-group {
  margin-top: 8px;
  display: flex;
  justify-content: end;
}

.end{
  margin-bottom: 85px;
}
</style>
