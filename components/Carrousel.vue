<template>
  <div class="container mx-auto px-4 overflow-x-scroll flex">
    <div class="pet-card w-full" v-for="pet in pets" :key="pet.id">
      <div
        class="w-full h-full rounded-md border mx-auto overflow-hidden hover:border-primary cursor-pointer"
      >
        <div class="pet-author px-4 py-3">
          <div class="flex items-center">
            <div class="w-8 h-8 rounded-full mr-2 border">
              <img
                class="w-8 h-8 object-cover"
                src="https://www.petz.com.br/blog/wp-content/uploads/2020/06/animais-com-sindrome-de-down-pet.jpg"
              />
            </div>
            <div class="text-sm">
              <p class="text-gray-800 text-md font-semibold">
                Gustavo Quinalha
              </p>
            </div>
          </div>
        </div>

        <div
          class="bg-cover bg-center w-full h-56 flex flex-col"
          :style="`background-image: url('https://www.petz.com.br/blog/wp-content/uploads/2020/06/animais-com-sindrome-de-down-pet.jpg')`"
        >
          <div class="flex">
            tag
            <!-- <UiChip primary small class="m-3">{{ race }}</UiChip> -->
          </div>

          <div class="flex flex-row-reverse m-3 mt-auto">
            <span
              class="pet-size-actived transition h-10 w-10 flex items-center justify-center bg-white text-primary rounded-full hover:bg-primary hover:text-white"
            >
              <!-- <IconLike class="w-8 h-8 rounded-full p-1" /> -->
              icon
            </span>
          </div>
        </div>

        <div class="px-4 pt-4 mb-3">
          <div class="font-semibold text-base text-gray-800">
            <span class="inline-block capitalize"> Doguineo </span>
            <span class="inline-block text-gray-500 font-medium text-base">
              - Marialva
            </span>
          </div>
        </div>
        <div class="flex justify-between">
          <div class="flex items-center justify-center size-wrapper">
            <span class="pet-size-actived">P</span>
            <span>M</span>
            <span>G</span>
          </div>

          <div class="flex items-center justify-center px-2">
            <svg-icon class="h-4 w-5 mr-1" name="pets/masc" />
            <p class="text-base whitespace-no-wrap">Macho</p>
          </div>
          <!-- <div class="flex items-center justify-center px-2">
          <svg-icon class="h-4 w-5 mr-1" name="pets/fem" />
          <p class="text-base whitespace-no-wrap">Fêmea</p>
        </div> -->

          <div class="flex items-center justify-center">
            <svg-icon class="h-4 w-5 mr-1" name="calendar" />
            <p class="text-base whitespace-no-wrap">2 Anos</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import { mapActions } from "vuex";
export default {
  data() {
    return {
      owner: {},
      avatar: "",
      race: "",
      name: "",
      city: "",
      size: "",
      sex: "",
      pets: [
        {
          id: 1,
          name: "joao",
        },
        {
          id: 1,
          name: "joao",
        },
        {
          id: 1,
          name: "joao",
        },
        {
          id: 1,
          name: "joao",
        },
        {
          id: 1,
          name: "joao",
        },
        {
          id: 1,
          name: "joao",
        },
      ],
    };
  },
  // computed: {
  //   petAge() {
  //     let date;

  //     if (this.pet.info && this.pet.info.birthdate) {
  //       date = this.$moment(new Date(this.pet.info.birthdate), "YYYYMMDD")
  //         .fromNow()
  //         .replace("há", "");
  //     }

  //     return date;
  //   },
  //   coverUrl() {
  //     const url = this.pet?.owner?.avatar;
  //     return url;
  //   }
  // },
  // props: {
  //   pet: {
  //     type: Object,
  //     default: () => ({
  //       info: {},
  //       owner: {},
  //       health: {}
  //     })
  //   }
  // },
  // methods: {
  //   ...mapActions({
  //     fetchPublicUserById: "user/fetchPublicUserById"
  //   })
  // },
  // mounted() {
  //   this.avatar = this.pet.avatar;
  //   this.race = this.pet.race;
  //   this.name = this.pet.name;
  //   this.city = this.pet.city;
  //   this.size = this.pet.size;
  //   this.sex = this.pet.sex;

  //   // if (this.pet && this.pet.info) {
  //   // }

  //   // if (this.pet.user_id) {
  //   //   this.fetchPublicUserById({ id: this.pet.user_id })
  //   //     .then(user => {
  //   //       this.owner = user
  //   //     })
  //   // }
  // },
  // updated() {
  //   if (this.pet && this.pet.info) {
  //     this.avatar = this.pet.info.avatar;
  //     this.race = this.pet.info.race;
  //     this.name = this.pet.info.name;
  //     this.city = this.pet.info.city;
  //     this.size = this.pet.info.size;
  //     this.sex = this.pet.info.sex;
  //   }
  // }
};
</script>

<style scoped>
.pets {
}
</style>
