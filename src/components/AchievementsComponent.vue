<template>
    <div class="achievements-container">
        <div 
            v-for="(achievement, index) in achievements" 
            :key="index" 
            :class="['achievement', { 'left': index % 2 === 0, 'right': index % 2 !== 0 }]">
            <h3>{{ achievement.title }}</h3>
            <p>{{ achievement.description }}</p>
            <p>Points: {{ achievement.points }}</p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            achievements: [
                { title: "First Achievement", description: "Description for the first achievement", points: 10 },
                { title: "Second Achievement", description: "Description for the second achievement", points: 20 },
                { title: "Third Achievement", description: "Description for the third achievement", points: 30 },
                // ... add as many achievements as you like
            ],
        };
    },
};
</script>

<style scoped>
.achievements-container {
    display: flex;
    flex-direction: column;
    align-items: center; /* This ensures that the flex items are centered in the container */
}

.achievement {
    border: 1px solid #ccc;
    border-radius: 5px;
    margin-bottom: 20px;
    padding: 10px;
    max-width: 80%; /* This restricts the width of the achievement boxes */
    margin-left: 20%;
    margin-right: 20%;
    background-color: #f5f5f5; /* Pastel white background color */
}

.left {
    align-self: flex-start;
    margin-right: auto; /* This will push the box to the left, maintaining the margin on the right */
}

.right {
    align-self: flex-end;
}

/* Responsive styles */
@media (max-width: 768px) {
    .achievement {
        max-width: 90%; /* Adjust the width for smaller screens */
        margin-left: 5%;
        margin-right: 5%;
    }
}
</style>
