<template>
    <div id="contact">
        <!-- <div id="contact">
            <img src="Assets/font-images/Contact font image.png" alt="Contact font image" height="110px" width="220px"
                class="mx-auto d-block m-5 image-fluid" loading="lazy">
        </div> -->
        <div class="container text-center bg-transparent mt-4 pt-5">

            <form action="https://formspree.io/f/myyvjoyz" method="post">
                <!--NAME-->
                <div class="form-outline mb-2 w-50 mx-auto">
                    <input type="text" name="name" id="form4Example1" class="form-control" required>
                    <label class="form-label" for="form4Example1">name</label>
                </div>

                <!--EMAIL-->
                <div class="form-outline mb-2 w-50 mx-auto">
                    <input type="email" name="email" id="form4Example2" class="form-control" required>
                    <label class="form-label" for="form4Example2">email</label>
                </div>

                <!--NUMBER-->
                <div class="form-outline mb-2 w-50 mx-auto">
                    <input type="text" name="contact" id="form4Example2" class="form-control" required>
                    <label class="form-label" for="form4Example2">contact</label>
                </div>
                <!--SHARE REFER-->
                <select class="form-select form-select-sm mb-1 w-50 mx-auto"
                    aria-label=".form-select-sm example">
                    <option selected>Topics:</option>
                    <option value="1">Business</option>
                    <option value="2">Personal</option>
                    <option value="3">Site issues / Suggestions</option>
                    <option value="3">Other</option>
                </select>

                <!--MESSAGE-->
                <div class="form-outline mb-1 w-50 mx-auto">
                    <textarea class="form-control" name="message" id="form4Example3" rows="4" required></textarea>
                    <label class="form-label" for="form4Example3">message</label>
                </div>
                <!--UPLOAD-->
                <div class="input-group mb-1 text-center w-50 mx-auto">
                    <label class="input-group-text mx-auto" for="inputGroupFile01">send</label>
                    <input type="file" class="form-control text-center" id="inputGroupFile01">
                </div>
                <!--SHARE REFER-->
                <select class="form-select form-select-sm text-center w-50 mx-auto"
                    aria-label=".form-select-sm example">
                    <!-- <option selected>How did you find this page?</option> -->
                    <!--text was too long to reduce text size to look good, so i made a label beneath the box (How did you find this page?)-->

                    <option value="1">Options</option>
                    <option value="2">Github</option>
                    <option value="3">Third Party</option>
                    <option value="4">Internet Search</option>
                    <option value="4">Other</option>
                </select>
                <label class="form-label" for="form4Example3">How did you find this page?</label>

                <br>

                <!--SUBMIT BUTTON-->
                <button type="submit" class="btn btn-outline-light mb-2">Send</button>
            </form>
        </div>
    </div>
</template>

<script>
</script>

<style scoped>
.btn:hover{
    background-color: #D2D79F;
}

#contact{
    margin-bottom: 40px;
}

@media screen and (max-width: 400px) {
    #contact{
    margin-bottom: 100px;
    }
}
/* .form-label{
  text-shadow: 4px 4px 4px rgb(0, 0, 0);
} */

/* form color */
/* custom form input colors and styling */
.form-control:focus {
  background-color: transparent;
  border-color: rgb(66, 133, 91);
  color: rgb(255, 255, 255);
  box-shadow: inset 0 1px 1px rgb(66, 133, 91), 0 0 8px rgb(210, 215, 159);
  transition: 5s;
}
.form-label:focus{
 background-color: rgba(255, 255, 255, 0.454);
}
.form-select:focus{
 background-color: rgba(255, 255, 255, 0.454);
 border-color: rgb(66, 133, 91);
  box-shadow: inset 0 1px 1px rgb(66, 133, 91), 0 0 8px rgb(210, 215, 159);
  transition: 5s
}
</style>