<template>
  <div>
    <div class="container" id="classCourse">
      <div class="row">
        <div class="col-sm-12">
          <h2 class="text-center text-info mb-5">Classroom Courses</h2>
          <p class="text-center">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam atque eius est eveniet magnam. Adipisci aliquid, aspernatur, enim facilis in ipsa ipsam mollitia, nobis nulla quis quisquam ratione recusandae rerum?</p>
          <h4 class="text-center font-weight-bold mt-4 text-muted mb-5">This month's available courses:</h4>
        </div>
      </div>
    </div>
    <div class="container-fluid bg-info py-4">
      <div class="row">
        <div class="col-md-6 my-4"  v-for="classCourse in classCourses">
          <div class="shadow h-100 bg-white">
            <div class="card-body">
              <table>
                <tr>
                  <td valign="top" class="text-center">
                    <h6 class="font-weight-bold bg-info text-white px-3 py-2 mr-3 mt-1 rounded">
                      {{ classCourse.month }}
                      <br/>
                      {{ classCourse.date }}
                    </h6>
                  </td>
                  <td>
                    <table>
                      <tr>
                        <td>
                          <h5 class="font-weight-bold text-info">{{ classCourse.title }}</h5>
                          <p class="mb-0 text-justify"><b>Course Detail:</b> {{ classCourse.description }}</p>
                          <p class="mb-0"><b>Location:</b> {{ classCourse.location }}</p>
                          <p><b>Time:</b> {{ classCourse.time }}</p>
                          <button @click="showForm" class="btn btn-sm btn-info " data-toggle="modal" :data-target="'#courseModal'+classCourse.id">Ask more info about this course</button>
                        </td>
                        <!--modal-->
                        <td class="modal fade" :id="'courseModal'+classCourse.id" aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
                          <div class="modal-dialog modal-dialog-centered modal-sm" role="document">
                            <div class="modal-content">
                              <form>
                                <div class="modal-body mt-4">
                                  <div class="form-group">
                                    <input type="text" class="form-control shadow-none" placeholder="Your name">
                                  </div>
                                  <div class="form-group">
                                    <input type="email" class="form-control shadow-none" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Email address">
                                  </div>
                                  <div class="form-group">
                                    <textarea class="form-control shadow-none" name="" id="" rows="3" placeholder="Your queries"></textarea>
                                  </div>
                                </div>
                                <div class="modal-footer border-0">
                                  <button type="button" class="btn btn-outline-danger" data-dismiss="modal">Close</button>
                                  <button type="submit" class="btn btn-outline-info">Submit</button>
                                </div>
                              </form>
                            </div>
                          </div>
                        </td>
                        <!--modal-->
                      </tr>
                    </table>
                  </td>
                </tr>
              </table>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ClassroomCourse",
  data () {
    return {
      classCourses: [
        {
          id: 1,
          title: 'Lorem ipsum dolor sit amet',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          month: 'Mar',
          date: '7',
          location: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          time: '9.30 AM'
        },
        {
          id: 2,
          title: 'Lorem ipsum dolor sit amet',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          month: 'Mar',
          date: '17',
          location: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          time: '10.00 AM'
        },
        {
          id: 3,
          title: 'Lorem ipsum dolor sit amet',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          month: 'Mar',
          date: '23',
          location: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          time: '11.00 AM'
        },
        {
          id: 4,
          title: 'Lorem ipsum dolor sit amet',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
          month: 'Mar',
          date: '28',
          location: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          time: '9.30 AM'
        }
      ]
    }
  }
}
</script>

<style scoped>
  .bg-class
  {
    background-image: url("../../static/images/Cuerda (1).jpg");
    background-repeat: no-repeat;
    background-size: cover;
  }
  .bg-class-overlay
  {
    background-color: rgba(23, 162, 184, .9);
    background-repeat: no-repeat;
  }
  input, textarea
  {
    border: 1px solid #17a2b8;
  }
  .modal-content
  {
    border: 3px solid #17a2b8;
  }
</style>
