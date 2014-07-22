//set global options
$(document).modal({
    easing : 'easeInOutBounce',
    speed : 600,
    animation : 'top',
    position 'center',
    overlayClose : true,
    on : 'click'
});
 
//per modal options, will use global options we set above
$('.clickMe').modal({
    target : '#modal1'
});
 
//override global options for this modal
$('.mouseover').modal({
    target : '#modal2',
    animation : 'zoom',
    position : '10px auto', //top 10px left auto
    easing : 'easeOutElastic',
    on : 'mouseenter',
    overlayClose : false,
    overlayColor : 'red',
    overlayOpacity : 0.5
    close : '.closeMe'
});
