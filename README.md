# Digital-clock 
function formatTime(time) {
    return time < 10 ? "0" + time : time;
  }
  
  function displayTime() {
    var currentTime = new Date();
    var hours = formatTime(currentTime.getHours());
    var minutes = formatTime(currentTime.getMinutes());
    var seconds = formatTime(currentTime.getSeconds());
    
    var formattedTime = hours + ":" + minutes + ":" + seconds;
    console.log(formattedTime);
  
    setInterval(displayTime, 3000); // Update every 3 seconds
  }
  
  displayTime();
  
