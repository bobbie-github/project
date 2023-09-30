<template>
  <div class="card-container relative overflow-hidden hover:shadow-lg transition">
    <div class="card-content">
      <img
          :src="imageSrc"
          alt="Card Image"
          class="w-full h-auto transition-transform transform hover:scale-110"
      />

      <div class="flex flex-col items-center">
        <img
            src="src/assets/Icons-20230930T071855Z-001/Icons/Frame 30.png"
            alt="Image 1"
            class="mb-4"
        />
        <img
            src="https://via.placeholder.com/300x200"
            alt="Image 2"
            class="mb-4"
        />
        <img
            src="https://via.placeholder.com/300x200"
            alt="Image 3"
            class="mb-4"
        />
      </div>
    </div>
    <div class="card-details absolute inset-0 flex items-center justify-center opacity-0 hover:opacity-100 transition">
      <div class="text-white text-center">
        <h3 class="text-lg font-bold">{{ title }}</h3>
        <p>{{ description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imageSrc: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
.card-container {
  width: 500px; /* Adjust the width as needed */
  height: 600px; /* Adjust the height as needed */
}

.card-content {
  position: relative;
}

.card-details {
  background-color: rgba(0, 0, 0, 0.8);
  padding: 20px;
}
</style>
