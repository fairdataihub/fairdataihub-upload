<script setup>
import uploadcare from "uploadcare-widget/uploadcare.lang.en.min.js";
import uploadcareTabEffects from "uploadcare-widget-tab-effects/dist/uploadcare.tab-effects.lang.en.min.js";

uploadcare.registerTab("preview", uploadcareTabEffects);
</script>

<template>
  <div>
    <h1 style="padding-bottom: 10px; margin: 0; font-size: 25px">
      Upload files for the FAIR Data Innovations Hub
    </h1>
    <p style="padding-bottom: 20px; margin: 0; color: darkslategrey">
      Your files will automatically start uploading as soon as you select them.
    </p>

    <input
      type="hidden"
      role="uploadcare-uploader"
      data-public-key="46d327bc8ff444a76df0"
      data-multiple="true"
      data-tabs="file camera url gdrive dropbox onedrive box huddle"
      data-effects="enhance, flip, crop, rotate, blur, grayscale, sharp, mirror, invert"
    />
  </div>
</template>
