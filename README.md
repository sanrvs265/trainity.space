# trainity.space

##// Here You can type your custom JavaScript...//weight autosave 100items
$(document).ready(function() {
  $("div#tabWeight_length select").val("100").change();
window.onload = function() {
  window.confirm = function() {
    var realConfirm = window.confirm;
    window.confirm = realConfirm;
    return true;
  }
}(10000);
  var butEl = document.getElementsByClassName('saveWeight'),
    count = butEl.length;
  for (i = 0; i < count; i++) {
    butEl[i].click(); 
  }
  if (document.all !== undefined) {
   var items = document.all;
 } else {
   var items = document.getElementsByTagName("*");
 };
 for (var i = 0; i < items.length; ++i) {
   if (items[i].textContent.includes("Enter Weight")) {
     console.log("success");
     items[i].click();
   }
 }
