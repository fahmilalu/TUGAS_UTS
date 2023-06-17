<script>
export default {
  props: ["id"],
  data() {
    return {
      data_images: [
        {
          id: 1,
          logo_name: "PERSIJA",
          logo_file: "persija.png",
          palyed: 8,
          scores: 4,
          lose: 0,
          rating: 5,
        },
        {
          id: 2,
          logo_name: "AREMA",
          logo_file: "arema.png",
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 3,
          logo_name: "PERSIB BANDUNG",
          logo_file: "persib.png",
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 4,
          logo_name: "PERSEBAYA",
          logo_file: "persebaya.png",
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 5,
          logo_name: "BARITO PUTERA",
          logo_file: "barito.png",
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 6,
          logo_name: "RANS FC",
          logo_file: "rans.png",
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 7,
          logo_name: "PSM MAKASAR",
          logo_file: "psm.png",
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 8,
          logo_name: "BALI UNITED",
          logo_file: "bali.png",
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 9,
          logo_name: "DEWA UNITED",
          logo_file: "dewa.png",
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 10,
          logo_name: "MADURA UNITED",
          logo_file: "madura.jpg",
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
      ],
    };
  },
};
</script>
<template>
  <div class="container">
    <div v-for="data_images in data_images" class="col">
      <div v-if="data_images.id == id">
        <div class="mt-2 mx-auto" style="width: 18rem">
          <img
            :src="'/src/assets/logo_bola/' + data_images.logo_file"
            class="rounded mx-auto d-block"
            alt="404"
          />
          <div class="card-body">
            <h5 class="text-center mt-2">{{ data_images.logo_name }}</h5>
          </div>
        </div>

        <div class="row row-cols-1 row-cols-md-4 g-4 mt-3">
          <div class="col">
            <div class="card shadow-sm">
              <div class="card-body">
                <h5 class="card-title">
                  Played <br />
                  {{ data_images.palyed }}
                </h5>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card shadow-sm">
              <div class="card-body">
                <h5 class="card-title">
                  Scores <br />
                  {{ data_images.scores }}
                </h5>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card shadow-sm">
              <div class="card-body">
                <h5 class="card-title">
                  Lose <br />
                  {{ data_images.lose }}
                </h5>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card shadow-sm">
              <div class="card-body">
                <h5 class="card-title">
                  Rating <br />
                  {{ data_images.rating }}
                </h5>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
img {
  width: 160px;
  height: 160px;
}
h5 {
  text-align: center;
}
</style>
