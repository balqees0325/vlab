<template>
  <div></div>
  <!-- <div class="page-Container">
    <div class="row">
      <div class="col-md-6">
        <p class="page-title">Physical Sciences</p>
        <p>
          But i must explain to you how all this mistaken idea of denouning
          pleasure and praising pain was born and i will
        </p>

        <div>
          <p class="instructors">Contributing Instructors</p>
          <p class="instructors-name">
            Carlos Zenzuke Albarran, Director and motion graphe
          </p>
        </div>
        <div class="view-practicals">
          <p class="view-Practical_text">
            View Practicals<span class="fa fa-arrow-down"></span>
          </p>
        </div>
      </div>
      <div class="col-md-6 side">
        <div class="expect">
          <p class="what-to-expect-text">What to expect</p>
          <div class="expect-content">
            <div v-for="x in 15" :key="x">
              <label class="container">
                1
                <input type="checkbox" checked="checked" />
                <span class="checkmark"></span>
              </label>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="input-row">
      <div class="col-md-6">
        <p>V-lab Practicals</p>
      </div>
      <div class="col-md-6">
        <div class="input-group">
          <div class="input-container">
            <input
              type="text"
              class="form-control input-bgc"
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

    <div class="vlab-practicals">
      <div class="container mt-5 mb-12">
        <div class="row">
          <div class="col-md-12">
            <ul class="timeline">
              <li class="child" v-for="x in 3" :key="x">
                <div class="col-md-10">
                  <div>
                    <span class="text">100 level</span>
                    <span class="text">Phy117</span>
                    <span class="text">100 level</span>
                  </div>
                  <h3 class="practical-title">virtual optics</h3>
                  <span style="font-size: 14px"
                    >Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                    Tenetur</span
                  >
                  <div class="practical-desc">
                    <span>12 Practicals</span>
                    <span>Lectures</span>
                    <span>Dr.Shamsu Laika</span>
                    <span>Dr.Shamsu Laika</span>
                  </div>
                </div>
                <div class="col-md-2">
                  <div class="bttn-container">
                    <button class="btn btn-secondary" type="submit">
                      <i class="fa fa-plus"></i>Add to Lab
                    </button>
                  </div>
                  <div>
                    <p class="md-size">More Details</p>
                  </div>
                </div>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>

    <div class="view-practicals-box"></div>
  </div> -->
</template>
<script>
export default {
  name: "ViwCourse",
};
</script>
<style scoped>
.timeline{
  margin-top:10px
}
.text{
  background-color: #d4d9df; 
  padding: 8px; 
  border-radius: 10px; 
  font-size: 16px;
}
.practical-desc {
  display: flex; 
  justify-content: space-between;
  width: 52%;
  font-size: 16px;
  padding: 8px 0;
}

.col-md-10 {
  display: flex;
  flex-direction: column;
  height: 8rem;
  
}

.col-md-2 {
  display: flex;
  flex-direction: column;
  justify-content:space-around;
}

.practical-title {
  font-weight: bolder;
  padding-top: 10px;
  text-transform: capitalize;
}

.child {
  background-color: #fff;
  margin-bottom: 30px;
  margin-top:10px;
  border-radius: 0.5rem;
  padding: 10px;
  height: 10rem;
  display: flex;
  justify-content: space-between;
}
ul.timeline {
  list-style-type: none;
  position: relative;
}
ul.timeline:before {
  content: " ";
  background: #d4d9df;
  display: inline-block;
  position: absolute;
  left: 29px;
  width: 2px;
  height: 100%;
  z-index: 400;
}
ul.timeline > li {
  margin: 0px 0;
  padding-left: 20px;
  margin-bottom: 10px;
}
ul.timeline > li:before {
  content: " ";
  background: white;
  display: inline-block;
  position: absolute;
  border-radius: 50%;
  border: 3px solid #0b0524;
  left: 20px;
  width: 20px;
  height: 20px;
  z-index: 400;
}

.vlab-practicals {
  width: 100%;
  background-color: #ebeaef;
  max-height: 700px;
  border-radius: 2.5rem;
  
}
.instructors {
  color: #959399;
  margin-bottom: 0%;
}
.view-practicals {
  width: 95%;
  background-color: #ebeaef;
  height: 200px;
  border-radius: 2rem;
  margin-top: 55px;
  display: flex;
}
.view-practicals-box {
  width: 12%;
  background-color: #adaabb;
  height: 150px;

  position: absolute;
  z-index: 1;
  border-radius: 2.5rem;
  right: 55%;
  top: 38%;
}
.view-Practical_text {
  align-self: flex-end;
  padding-left: 20px;
}
.fa {
  padding-left: 5px;
}

.side {
  display: flex;
  justify-content: flex-end;
}
.expect {
  width: 55%;
  background-color: #ebeaef;
  height: 300px;
  border-radius: 2rem;
  margin-top: 55px;
}
.what-to-expect-text {
  padding-left: 20px;
  padding-top: 20px;
  font-weight: bold;
  color: #0b0524;
}
.expect-content {
  width: 90%;
  overflow-x: hidden;
  overflow-y: scroll;
  scrollbar-color: #0b0524 #bebebe;
  scrollbar-width: thin;
  max-height: 220px;
  margin-left: 15px;
}
.input-row {
  margin-top: 20px;
}
.md-size{
  font-size: 16px;
}
</style>