
/* top search form
================================================== */
jQuery(document).ready(function() {
	jQuery('.search-wrapper.top .submit').click(function(e){
		if(jQuery('.search-wrapper.top').width()==45) {
			e.preventDefault();
			var a = jQuery('#main-nav').width();
			var b = jQuery('#main-nav > li').size();
			var e = jQuery('#main-nav > li > a > span.sf-sub-indicator').size();
			a = a-740;
			if (a>0) {
			b = a/b;
			var c = Math.round(Math.round(b)/2);
			c = e+7-c;
			var d = 0;
			}
		jQuery(this).parent().addClass("open");
		jQuery(this).parent().animate({width:"218px"},300);
		jQuery(this).siblings('input').val('').focus().select();
		jQuery(this).parent().parent().siblings('#main-nav').find('> li > a > .left > .right > .middle').animate({'padding-left':c,'padding-right':c},300);
		jQuery(this).parent().parent().siblings('#main-nav').find('> li > a > .sf-sub-indicator').animate({'width':d},300);
		return false;
		}
		if(jQuery(this).siblings('.text').val()=='') {
		return false;
		}
	});
	jQuery(".search-wrapper.top").click(function(){
	   if (event.stopPropagation){
		   event.stopPropagation();
	   }
	   else if(window.event){
		  window.event.cancelBubble=true;
	   }
	});
	jQuery("html").click(function(){
		if (jQuery('.search-wrapper.top').width() == 218) {
		jQuery(this).find('.search-wrapper.top').removeClass("open");
		jQuery(this).find('.search-wrapper.top').animate({width:'45px'},300);
		jQuery(this).find('#main-nav > li > a > .left > .right > .middle').animate({'padding-left':'10px','padding-right':'10px'},300);
		jQuery(this).find('#main-nav > li > a.sf-with-ul > .left > .right > .middle').animate({'padding-right':'1.25em'},300);
		jQuery(this).find('#main-nav > li > a > .sf-sub-indicator').animate({width:'9px'},300);
		}
	});
});