<template>
  <div class="total">
    <div class="sun">
      <transition
        class="sunT"
        appear
        @before-enter="beforeEnterSun"
        @enter="enterSun"
      >
        <img src="./assets/sun.png" alt="sun" />
      </transition>
    </div>
    <div class="clouds">
      <transition
        class="cloud"
        appear
        @before-enter="beforeEnterC"
        @enter="enterC"
      >
        <img src="./assets/cloud.png" alt="cloud" />
      </transition>
      <transition
        class="cloud"
        appear
        @before-enter="beforeEnterC1"
        @enter="enterC1"
      >
        <img src="./assets/cloud.png" alt="cloud" />
      </transition>
      <transition
        class="cloud"
        appear
        @before-enter="beforeEnterC2"
        @enter="enterC2"
      >
        <img src="./assets/cloud.png" alt="cloud" />
      </transition>
      <transition
        class="cloud"
        appear
        @before-enter="beforeEnterC3"
        @enter="enterC3"
      >
        <img src="./assets/cloud.png" alt="cloud" />
      </transition>
      <transition
        class="cloud"
        appear
        @before-enter="beforeEnterC4"
        @enter="enterC4"
      >
        <img src="./assets/cloud.png" alt="cloud" />
      </transition>
      <transition
        class="cloud"
        appear
        @before-enter="beforeEnterC5"
        @enter="enterC5"
      >
        <img src="./assets/cloud.png" alt="cloud" />
      </transition>
    </div>
    <div class="rainbow">
      <transition class="rainbowT" appear @before-enter="beforeEnterR" @enter="enterR">
        <img src="./assets/rainbow.png" alt="rainbow" />
      </transition>
    </div>
    <div class="mounts">
      <transition
        class="mount"
        appear
        @before-enter="beforeEnter"
        @enter="enter"
      >
        <img src="./assets/mount.png" alt="mount" />
      </transition>
      <transition
        class="mount"
        appear
        @before-enter="beforeEnter1"
        @enter="enter1"
      >
        <img src="./assets/mount.png" alt="mount" />
      </transition>
      <transition
        class="mount"
        appear
        @before-enter="beforeEnter2"
        @enter="enter2"
      >
        <img src="./assets/mount.png" alt="mount" />
      </transition>
      <transition
        class="mount"
        appear
        @before-enter="beforeEnter3"
        @enter="enter3"
      >
        <img src="./assets/mount.png" alt="mount" />
      </transition>
      <transition
        class="mount"
        appear
        @before-enter="beforeEnter4"
        @enter="enter4"
      >
        <img src="./assets/mount.png" alt="mount" />
      </transition>
      <transition
        class="mount"
        appear
        @before-enter="beforeEnter5"
        @enter="enter5"
      >
        <img src="./assets/mount.png" alt="mount" />
      </transition>
    </div>
  </div>
</template>

<script>
import gsap from "gsap";
export default {
  methods: {
    beforeEnter(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(100px)";
    },
    beforeEnter1(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(100px)";
    },
    beforeEnter2(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(100px)";
    },
    beforeEnter3(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(100px)";
    },
    beforeEnter4(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(100px)";
    },
    beforeEnter5(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(100px)";
    },
    beforeEnterC(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(-10px)";
    },
    beforeEnterC1(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(-100px)";
    },
    beforeEnterC2(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(-100px)";
    },
    beforeEnterC3(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(-100px)";
    },
    beforeEnterC4(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(-100px)";
    },
    beforeEnterC5(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(-100px)";
    },
    beforeEnterR(el) {
      el.style.opacity = "0";
    },
    beforeEnterSun(el) {
      el.style.opacity = "0";
      el.style.transform = "translateY(200px)";
    },
    enter(el) {
      gsap.to(el, {
        duration: 1.2,
        stagger: 0.1,
        ease: "bounce.out",
        delay: 6,
        y: 0,
        opacity: 1,
      });
    },
    enter1(el) {
      gsap.to(el, {
        duration: 0.8,
        stagger: 0.1,
        delay: 3,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enter2(el) {
      gsap.to(el, {
        duration: 0.8,
        stagger: 0.1,
        delay: 2,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enter3(el) {
      gsap.to(el, {
        duration: 0.8,
        stagger: 0.1,
        delay: 4,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enter4(el) {
      gsap.to(el, {
        duration: 0.8,
        stagger: 0.1,
        delay: 5,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enter5(el) {
      gsap.to(el, {
        duration: 0.8,
        stagger: 0.1,
        delay: 1,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enterC(el) {
      gsap.to(el, {
        duration: 0.6,
        stagger: 0.1,
        delay: 7,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enterC1(el) {
      gsap.to(el, {
        duration: 0.6,
        stagger: 0.1,
        delay: 10,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enterC2(el) {
      gsap.to(el, {
        duration: 0.6,
        stagger: 0.1,
        delay: 8,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enterC3(el) {
      gsap.to(el, {
        duration: 0.6,
        stagger: 0.1,
        delay: 9,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enterC4(el) {
      gsap.to(el, {
        duration: 0.6,
        stagger: 0.1,
        delay: 12,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enterC5(el) {
      gsap.to(el, {
        duration: 0.6,
        stagger: 0.1,
        delay: 11,
        ease: "bounce.out",
        y: 0,
        opacity: 1,
      });
    },
    enterSun(el) {
      gsap.to(el, {
        duration: 8,
        stagger: 0.1,
        delay: 13,
        ease: true,
        y: 0,
        opacity: 1,
      });
    },
    enterR(el) {
      gsap.to(el, {
        duration: 4,
        stagger: 0.1,
        delay: 16,
        ease: true,
        y: 0,
        opacity: 1,
      });
    },
  },
};
</script>