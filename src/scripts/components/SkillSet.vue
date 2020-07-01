<template>
  <section class="skillset">
    <div class="container">
      <div class="row">
        <div class="col-md-3 d-flex justify-content-lg-center align-items-center order-md-0 order-1 py-lg-0 py-4">
          <div class="d-block mx-auto skillset-inner">
            <div class="skillset-title h2">Front-End Developer</div>
            <div class="skillset-body">
              <p class="mb-0" v-for="(skill, index) in frontEndSkills" :key="index">{{skill}}</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 order-md-1 order-0 mb-lg-0 mb-4">
          <figure>
            <PieIcon />
          </figure>
        </div>
        <div class="col-md-3 d-flex justify-content-lg-center align-items-center order-md-2 order-2 py-lg-0 py-4">
          <div class="d-block mx-auto skillset-inner">
            <div class="skillset-title h2">Designer</div>
            <p class="mb-0" v-for="(skill, index) in designerSkills" :key="index">{{skill}}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SkillSet",
  data() {
    return {
      frontEndSkills: [
        "Programming",
        "Web development",
        "Cross-platform",
        "Page Optimization",
        "Drinking coffee",
        "Smashing keyboards",
        "Code isn't working, crying in front of my computer"
      ],
      designerSkills: [
        "UI/UX Design",
        "Responsive Design",
        "Minimal Design",
        "Copying and mixing ideas from other designers"
      ]
    };
  }
};
</script>