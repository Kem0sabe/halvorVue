<template>
    <nav>
        <ul>
            <li @click="scrollToSection('home')">Home</li>
            <li @click="scrollToSection('introduction')">Introduction</li>
            <li @click="scrollToSection('achievements')">Achievements</li>
            <li @click="scrollToSection('form')">Form</li>
        </ul>
    </nav>
</template>

<script>
export default {
    methods: {
        scrollToSection(sectionId) {
            const section = document.getElementById(sectionId);
            if (section) {
                section.scrollIntoView({ behavior: 'smooth' });
            }
        }
    }
}
</script>

<style scoped>
nav {
    background-color: #f8f8f8;
    padding: 10px;
    border-radius: 10px; /* Add this line */
}

ul {
    list-style-type: none;
    display: flex;
    justify-content: space-around;
}

li {
    cursor: pointer;
}
</style>
