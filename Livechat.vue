<template> 
<button type="button" class="btn btn-primary" id="liveToastBtn">Live Now</button>

<div class="toast-container position-fixed bottom-0 end-0 p-3">
  <div id="liveToast" class="toast" role="alert" aria-live="assertive" aria-atomic="true">
    <div class="toast-header">
      <img src="..." class="rounded me-2" alt="...">
      <strong class="me-auto">Cluidly Scipt</strong>
      <small>Live Now</small>
      <button type="button" class="btn-close" data-bs-dismiss="toast" aria-label="Close"></button>
    </div>
    <div class="toast-body">
      Hello Every one Your are Live in Chat Now in the session in the hole
    </div>
  </div>
</div>    

</template> 
<script>  
 const toastTrigger = document.getElementById('liveToastBtn')
 const toastLiveExample = document.getElementById('liveToast')

 if (toastTrigger) {
  const toastBootstrap = bootstrap.Toast.getOrCreateInstance(toastLiveExample)
  toastTrigger.addEventListener('click', () => {
    toastBootstrap.show()
  })
}
</script>