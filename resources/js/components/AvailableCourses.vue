<template>
  <div class="page-Container">
    <div class="input-row">
      <div class="col-md-6">
        <p>Available V-lab Courses</p>
      </div>
      <div class="col-md-6">
        <div class="input-group">
          <div class="input-container">
          <input
            type="text"
            class="form-control"
            placeholder="Search Courses"
          />
          </div>
          <div class="input-group-btn btn-container">
            <button class="btn btn-default" type="submit">
              <i class="fa fa-search"></i>
            </button>
          </div>
        </div>
      </div>
    </div>
    <div class="course-container">
      <div v-for="x in 8" :key="x" class="col-md-3">
        <div class="card" style="width: 100%;">
          
          <div class="card-body">
            <h5 class="card-title">
              <a href="/vewCourse" class="btn btn-light">Applied Sciences</a>
            </h5>
            <p class="card-text">Electrical Engineering</p>
            <p>Dr Shemsu Laika</p>

            <a href="#" class="card-link">
              <a href="#" class="card-link" style="float: left"
                ><span class="fa fa-windows"></span>32 Modules</a
              >
              <a href="#" class="card-link" style="float: right"
                ><span class="fa fa-user"></span>409 Students</a
              >
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AvalaibleCourses",
  props: ['image1'],
  mounted: function () {
   var $vm  = this;
  this.$nextTick(function () {
    // Code that will run only after the
    // entire view has been rendered
    console.log($vm.image1);
  })
}
 
};
</script>

<style scoped>

.card-link {
  color: #2f2651;
  font-size: 12px;
}
.h5 {
  font-size: 10px;
  color: #000;
}
.form-control {
  border-radius: 0.5rem;
  width: 40%;
  float: right;
  background-color: #eeeeef;
}
.col-md-6 {
  padding-left: 35px;
}
.btn-light {
  border-radius: 1rem;
  background-color: eeeeef;
}
.card-text {
  color: #2f2651;
  font-weight: bold;
}

.card-img-top {
  border-radius: 1rem;
}
.card {
  padding: 10px;
  background-color: #eeeeef;
  margin: 0 0 20px 0;
}



</style>