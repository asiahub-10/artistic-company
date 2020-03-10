<template>
    <div>
      <div class="container">
        <div class="row">
          <div class="col-sm-12">
            <h1 class="font-weight-bold header-font text-center text-info mb-3">Corsos</h1>
          </div>
        </div>
      </div>
      <classroom-course/>
      <online-course/>
    </div>
</template>

<script>
import Online from './OnlineCourse'
import ClassroomCourse from "./ClassroomCourse";

export default {
  name: "Course",
  components: {
    'classroom-course': ClassroomCourse,
    'online-course': Online
  },
  data () {
    return {

    }
  }
}
</script>

<style scoped>


</style>
