<template>
  <form data-abide novalidate>
    <div class="grid-container">
      <div class="grid-x">
        <div class="cell small-12">
          <div class="alert callout" data-abide-error style="display: none">
            <p><i class="fi-alert"></i>There are errors in your form.</p>
          </div>
        </div>
      </div>
    </div>
    <div class="grid-container">
      <div class="grid-x">
        <div class="cell small-12">
          <label
            >Email (Required)
            <input
              type="text"
              placeholder="hello@example.com"
              required
              pattern="email"
            />
            <span class="form-error" data-form-error-on="required"
              >This field is required.</span
            >
            <span class="form-error" data-form-error-on="pattern"
              >Invalid email.</span
            >
          </label>
        </div>
        <div class="cell small-12">
          <label
            >Password (Required)
            <input
              id="password"
              type="password"
              placeholder="chewieR2D2"
              required
            />
            <span class="form-error"> This field is required. </span></label
          >
        </div>
        <div class="cell small-12">
          <label
            >Re-enter Password (Required)
            <input
              type="password"
              placeholder="chewieR2D2"
              required
              pattern="alpha_numeric"
              data-equalto="password"
            />
            <span class="form-error" data-form-error-on="required"
              >This field is required.</span
            >
            <span class="form-error" data-form-error-on="equalTo"
              >Passwords don't match.</span
            ></label
          >
        </div>
        <div class="cell small-12">
          <button class="button" type="submit" value="Submit">Submit</button>
          <button class="button" type="reset" value="Reset">Reset</button>
        </div>
      </div>
    </div>
  </form>
</template>

<script>
/* eslint id-length: ["error", { "exceptions": ["$"] }] */
import $ from 'jquery'

const component = {
  mounted() {
    $(document).foundation()
  },
}

export default component
</script>
