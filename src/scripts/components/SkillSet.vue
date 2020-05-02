<template>
  <section class="skillset">
    <div class="container">
      <div class="row">
        <div class="col-md-3 d-flex justify-content-center align-items-center order-md-0 order-1">
          <div class="d-block">
            <div class="skillset-title h2">Front-End Developer</div>
            <div class="skillset-body">
              <p class="mb-0" v-for="(skill, index) in frontEndSkills" :key="index">{{skill}}</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 order-md-1 order-0">
          <figure>
            <PieIcon />
          </figure>
        </div>
        <div class="col-md-3 d-flex justify-content-center align-items-center order-md-2 order-2">
          <div class="d-block">
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
        "Cursing computers"
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