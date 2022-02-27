<template>
  <div class="contact">
    <div class="contact-container">
      <h2 class="contact-title">Contact Us</h2>
      <div class="label">Address</div>
      <div>101 S 200 E Suite 300</div>
      <div>Salt Lake City, UT 84111</div>
      <div class="label">Phone</div>
      <div>(801) 715-7141</div>
      <div class="label">Toll free number</div>
      <div>(800) 657-6363</div>
      <div class="spacer"></div>
    </div>
  </div>
</template>

<style>
.contact {
  display: flex;
  justify-content: center;
  padding: 20px 40px;
}
.contact-container {
  width: 100%;
  max-width: 800px;
}
.contact-title {
  margin-left: 20px;
  margin-bottom: 40px;
}
.label {
  font-weight: bold;
  margin-bottom: 10px;
  margin-top: 20px;
}
.spacer {
  height: 60px;
}
</style>
