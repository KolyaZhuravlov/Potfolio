<template>
  <div class="header-container">
    <div class="header-info">
      <h1>Hi, I'm Kolya <span class="hello"> 👋 </span></h1>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo eius laboriosam ratione
        corporis tempore facilis, laborum, debitis dolorem accusamus accusantium modi obcaecati?
      </p>
      <div class="header-btn">
        <button class="btn">Hire Me</button>
        <button class="download" @click="downloadFile">Download resume</button>
      </div>
    </div>

    <div class="header-img">
      <img src="/src/icons/IMG_4404.jpg" alt="kolya foto" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
    }
  },
  methods: {
    downloadFile() {
      const fileUrl = 'src/public/kolyazh.pdf'

      const link = document.createElement('a')
      link.href = fileUrl
      link.download = 'kolyazh.pdf'
      link.click()
    },
  },
}
</script>

<style scoped>
.header-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  padding: 20px;
}
.header-info {
  flex: 1;
  padding-right: 20px;
}
.header-img img {
  height: auto;
  width: 360px;
  border-radius: 50%;
  margin-right: 100px;
  margin-top: 50px;
}
.header-info {
  width: 700px;
  height: 500px;
  margin-top: 50px;
  text-align: center;
}
h1 {
  font-size: 40px;
  margin-top: 20px;
  font-weight: bold;
}
p {
  margin-top: 70px;
}
.btn {
  margin-top: 100px;
  margin-right: 20px;
  background-color: rgb(245 158 11);
  width: 140px;
  height: 50px;
  border-radius: 25px;
  font-weight: bold;
  transition: transform 0.3s ease;
}
.download {
  font-weight: bold;
  border-radius: 25px;
  color: rgb(245 158 11);
  border: 2px solid rgb(245 158 11);
  width: 220px;
  height: 50px;
  transition: transform 0.3s ease;
}
.btn:hover {
  transform: scale(1.05);
}
.download:hover {
  transform: scale(1.05);
}
.hello {
  animation-name: hello-animations;
  animation-duration: 2.1s;
  animation-iteration-count: infinite;
  transform-origin: 70% 70%;
  display: inline-block;
}
@keyframes hello-animations {
  0% {
    transform: rotate(0);
  }
  10% {
    transform: rotate(14deg);
  }
  20% {
    transform: rotate(-8deg);
  }
  30% {
    transform: rotate(14deg);
  }
  40% {
    transform: rotate(-4deg);
  }
  50% {
    transform: rotate(10deg);
  }
  60% {
    transform: rotate(0);
  }
  100% {
    transform: rotate(0);
  }
}

@media (max-width: 900px){
	.header-container {
    flex-direction: column; /* Размещаем элементы по вертикали */
    align-items: center; /* Центрируем все элементы */
    text-align: center;
  }

  .header-img img {
    width: 250px; /* Уменьшаем изображение на мобильных устройствах */
    margin-bottom: 20px; /* Добавляем отступ снизу */
  }
  .header-btn {
	margin-left: 20px;
  }

  .header-info {
    width: 100%; /* Занимаем всю ширину контейнера */
    text-align: center;
  }

  h1 {
    font-size: 30px;
  }

  p {
    font-size: 18px;
    margin-top: 20px; /* Уменьшаем отступ сверху */
  }

  .btn {
    margin-top: 20px;
	 width: 100px
  }

  .download {
    margin-top: 20px;
	 width: 180px;
  }
  img {
	align-items: center;
	display: flex;
	margin-left: 50px;
	margin-top: 20px;
  }
}

</style>
