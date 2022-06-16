<template>
  <section>
    <div class="container-sm">
      <h1>Make An Appointment</h1>
      <hr />
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi vitae
        temporibus harum, dicta neque cupiditate cumque voluptatem dolor,
        aspernatur eu
      </p>
      <div class="form">
        <form>
          <input type="text" placeholder="Name*" />
          <input type="email" placeholder="Email*" />
          <input type="tel" placeholder="Phone Number" />
          <input type="date" />
          <textarea rows="5" placeholder="How can we help?" ></textarea>
          <button type="submit">MAKE AN APPOINTMENT</button>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppointmentSection",
};
</script>

<style lang="scss" scoped>
section {
  display: flex;
  align-items: center;
  height: 90vh;
  text-align: center;
  color: lightgray;
  background-image: url("../../assets/img/make-an-appointment.jpg");
  background-size: cover;
  background-position: center;

  h1{
    font-weight: 400;
  }

  & form {
    margin-top: 40px;
    justify-content: center;
    display: flex;
    flex-wrap: wrap;
    gap: 20px;

    & > *:not(button[type="submit"]) {
      background: none;
      border: 1px solid var(--color-lightgrey);
      padding: 10px 10px;
      color: lightgray;
      

      &::placeholder {
        color: lightgray;
      }
    }

    input {
      width: calc(100% / 2 - 20px);
    }

    textarea {
      width: calc(100% - 20px);
      resize: none;
    }

    button{
        background-color: var(--primary-color);
        color:white;
        width: calc(100% - 20px);
        padding: 10px 0;
        border:none;

        &:hover{
            cursor: pointer;
        }
    }
  }
}
</style>