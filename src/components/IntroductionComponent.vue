<template>
  <div class="introduction">
    <div class="image-container">
      <img src="@/assets/halvor.jpg" alt="Person Image" class="person-image" />
    </div>
    <div class="text-container">
      <h1>Welcome to my personal website!</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
        consectetur, justo at aliquet tincidunt, mauris nisl ultrices purus,
        vitae consectetur nunc elit ac nunc. Sed euismod, nunc id aliquam
        aliquet, nunc elit tincidunt nunc, vitae consectetur nunc elit ac nunc.
      </p>
    </div>
  </div>
</template>

<style>
.introduction {
  display: flex;
  align-items: center;
}

.image-container {
  flex: 1;
}

.person-image {
  width: 100%;
  max-width: 300px;
  border-radius: 10px; /* Add this line to make the corners rounded */
}

.text-container {
  flex: 2;
  padding: 0 20px;
}

h1 {
  font-size: 24px;
  margin-bottom: 10px;
}

p {
  font-size: 16px;
  line-height: 1.5;
}
</style>
