# 
GSAP scrolling experiment demonstrates how to create scroll-based animations using the GSAP (GreenSock Animation Platform) library. 

In this particular example, we have a red box element that will fade in when it comes into view during scrolling.

The HTML structure consists of a container element that provides a height to enable scrolling and a box element that represents the animated element.

In the CSS, the container is given a height of 2000 pixels, which creates a scrollable area. The box is styled with a red background color, white text, and centered using absolute positioning.

The JavaScript code starts by importing the necessary GSAP modules, including the gsap and ScrollTrigger. The ScrollTrigger plugin is then registered using the gsap.registerPlugin() method.

Next, we select the box element using document.querySelector('.box') and create a GSAP animation using gsap.to(). The animation targets the box element and animates its opacity property from 0 to 1.

The scrollTrigger property is added to the animation options to define when the animation should be triggered. In this case, the trigger property is set to the box element itself, start is set to 'top 80%', and end is set to 'bottom 20%'. This means the animation will start when the top of the box is 80% in view and end when the bottom of the box is 20% in view.

The toggleActions property is set to 'play none none reset'. This means that when the box comes into view, the animation will play. Once it goes out of view, the animation will be reset to its initial state.

By combining GSAP's animation capabilities with the ScrollTrigger plugin, you can create engaging scroll-based effects and animations on your web pages.

Remember to include the GSAP library and the ScrollTrigger plugin in your project for this experiment to work successfully.
