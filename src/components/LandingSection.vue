<template>
    <div class="container">
<div class="row vh-100 align-items-center">
    <div class="col">
        <img
          src="https://nusaibah01.github.io/all-images/images/20240422_101945.jpg"
          alt="profile"
          class="img-fluid"
          loading="lazy"
        />
    </div>
    <div class="col">
        <div id="details">
            <h1 class="display-1" id="text">Nusaibah Charif</h1>
           <p v-if="title" id="text">
            I am an
            <span>{{ title}}</span>
        </p>
       <Spinner v-else />
        </div>
    </div>
</div>
    </div>
</template>