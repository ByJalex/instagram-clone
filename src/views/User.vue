<template>
  <div>
    <div class="header-home">
      <div class="header-home-son justify-between">
        <vs-avatar>
          <i class="bx bx-user-plus icons-header"></i>
        </vs-avatar>
        <div>josue_ayala27</div>
        <vs-avatar>
          <i class="bx bx-cog icons-header"></i>
        </vs-avatar>
      </div>
    </div>
    <div class="break"></div>
    <div class="content-profile">
      <div class="profile-edit">
        <div class="photo-profile">
          <vs-avatar size="70" circle>
            <i class="bx bx-user"></i>
          </vs-avatar>
        </div>
        <div class="name-edit">
          <p>josue_ayala27</p>
          <button class="btn-edit">Editar Perfil</button>
        </div>
      </div>
      <div class="break-2"></div>
      <div class="profile-description">
        <span class="name">J O S 📷</span>
        <br />
        <span>Tomo fotos y les pongo filtros de WhatsApp 😛</span>
        <span>
          Fotografias:
          <router-link to="/test">@josueayala27</router-link>
        </span>
        <br />
        <span>🚺 📷 🎨 🎵 💻</span>
      </div>
      <div class="profileStories">
        <div class="break-2"></div>
        <div class="content">
          <div class="icon-storie" v-for="index in 20" :key="index">
            <vs-avatar size="70" circle history>
              <i class="bx bx-user"></i>
            </vs-avatar>
            <div class style>
              <small class="userProfile">Featured</small>
            </div>
          </div>
        </div>
      </div>
      <div class="break-2"></div>
      <div class="line-bottom"></div>
      <div class="break-2"></div>
      <div class="info">
        <div class="item-info">
          <div>
            <div>
              <b>34</b>
            </div>
            <div>Publicaciones</div>
          </div>
        </div>
        <div class="item-info">
          <div>
            <div>
              <b>1,618</b>
            </div>
            <div>Seguidores</div>
          </div>
        </div>
        <div class="item-info">
          <div>
            <div>
              <b>90</b>
            </div>
            <div>Seguidos</div>
          </div>
        </div>
      </div>
      <div class="break-2"></div>
      <div class="line-bottom"></div>
      <div class="break-2"></div>
      <div class="items-icons">
        <i class="bx bx-grid-alt bx-sm"></i>
        <i class="bx bx-card bx-sm"></i>
        <i class="bx bx-tv bx-sm"></i>
        <i class="bx bx-collection bx-sm"></i>
        <i class="bx bx-purchase-tag bx-sm"></i>
      </div>
      <div class="break-2"></div>
      <div class="image-not-found">
        <div>
          <i class="bx bx-cloud-upload image-upload"></i>
          <p class="text">Subir tu primera foto</p>
        </div>
      </div>
    </div>

    <div class="end"></div>
  </div>
</template>