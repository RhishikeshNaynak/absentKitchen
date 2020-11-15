<template>
  <div>
    <div>
      <img
        class="relative hidden md:block"
        src="/assets/Background.svg"
        alt="Banenr Image"
      />
      <img
        class="relative block md:hidden"
        src="/assets/mobileBg.svg"
        alt="Banenr Image"
      />
    </div>
    <div class="logo flex justify-center">
      <img class="h-56 md:h-48 " src="/assets/LOGO.svg" />
    </div>
    <div class="para hidden  md:flex justify-center">
      <h1 class="text-4xl font-bold ">OPENING</h1>
      <img class="rotate  h-10 mt-3 mx-1" src="/assets/Pizza.svg" />
      <h1 class="text-4xl font-bold ">SOON</h1>
    </div>
    <!-- -------------mobile-------------- -->
    <div class="para block text-center md:hidden">
      <h1 class="abc text-5xl absolute z-50 font-bold ">
        OPENING
      </h1>
      <h1 class="abc text-5xl absolute pt-5 mt-40 z-50 font-bold  ">
        SOON
      </h1>
      <img class="rotate relative mt-10 mx-auto" src="/assets/Pizza.svg" />
    </div>

    <div class="para-txt text-xl md:text-lg flex justify-center">
      <div>
        <p class="md:pl-10">Our website is launching soon.</p>
        <p class="hidden md:flex">Be the first to know by subscribing today.</p>
        <p class="block text-center md:hidden">Be the first to know by</p>
        <p class="block text-center md:hidden">subscribing today.</p>
      </div>
    </div>
    <div class="notify hidden md:flex justify-center">
      <div class="p-8">
        <div class="bg-white flex  rounded-full ">
          <input
            class="rounded-l-full w-full  mx-5  text-gray-900 leading-tight focus:outline-none"
            id="E-mail"
            type="text"
            placeholder="E-mail"
          />

          <div class="">
            <button
              class="text-white rounded-full px-10 bg-orange-600  h-10 flex items-center justify-center"
            >
              Notify
            </button>
          </div>
        </div>
      </div>
    </div>

    <!-- -------------------for mobile-------------------- -->
    <div class="notify pt-5 md:hidden flex justify-center">
      <button
        class="btn text-yellow-400 rounded-full px-10 bg-none  h-10 flex items-center justify-center"
      >
        Notify Me!
      </button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.abc {
  position: absolute;
  text-align: center;
  width: 100%;
}
.logo {
  position: absolute;
  top: 10%;
  margin: auto;
  /* position: absolute; */
  /* top: 0; */
  left: 0;
  /* bottom: 0; */
  right: 0;
}
.para {
  position: absolute;
  top: 43%;
  color: yellow;
  margin: auto;
  left: 0;
  right: 0;
}
@media (max-width: 640px) {
  .para {
    position: absolute;
    top: 45%;
    color: yellow;
    margin: auto;
    left: 0;
    right: 0;
  }
}
.para-txt {
  position: absolute;
  top: 50%;
  color: yellow;
  margin: auto;
  left: 0;
  right: 0;
}

@media (max-width: 640px) {
  .para-txt {
    position: absolute;
    top: 82%;
    color: yellow;
    margin: auto;
    left: 0;
    right: 0;
  }
}
.notify {
  position: absolute;
  top: 55%;
  /* color: yellow; */
  margin: auto;
  left: 0;
  right: 0;
}

@media (max-width: 640px) {
  .notify {
    position: absolute;
    top: 95%;
    /* color: yellow; */
    margin: auto;
    left: 0;
    right: 0;
  }
}

.rotate {
  animation: rotation 5s infinite linear;
}

@keyframes rotation {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(359deg);
  }
}

.btn {
  border: 3px solid red;
  animation: color-change 2s infinite;
}

@-webkit-keyframes color-change {
  0% {
    border-color: red;
  }
  20% {
    border-color: orange;
  }

  40% {
    border-color: green;
  }
  60% {
    border-color: DarkBlue;
  }
  80% {
    border-color: purple;
  }
  100% {
    border-color: red;
  }
}
</style>
