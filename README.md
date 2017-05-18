##Useful tool to measure performance. Learn and use it for all future projects

```// User Timing API to the rescue again. Seriously, it's worth learning.
  // Super easy to create custom metrics.
  window.performance.mark("mark_end_frame");
  window.performance.measure("measure_frame_duration", "mark_start_frame", "mark_end_frame");
  if (frame % 10 === 0) {
    var timesToUpdatePosition = window.performance.getEntriesByName("measure_frame_duration");
    logAverageFrame(timesToUpdatePosition);
  }

##Who doesn't like delicious pizza?

This site supports [this quiz](https://www.udacity.com/course/viewer#!/c-ud860/l-4147498575/e-4154208580/m-4142388616) from Udacity's [Browser Rendering Optimization](http://udacity.com/ud860)

This pizzeria site is a performance nightmare. Record a timeline trace and watch the Forced Synchronous Layout warnings pop up. Can you make this site run at 60fps?
