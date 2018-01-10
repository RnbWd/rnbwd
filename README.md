
> how to make a rainbow in CSS

````
@include keyframes(rainbow) {
  from {
    @include filter(hue-rotate(0deg));
  }
  to {
    @include filter(hue-rotate(360deg));
  }
}

.main {
  @include animation(rainbow 10.0s linear infinite);
}

.rainbow {
  @include transform(translateZ(0));
  @include animation(rainbow 8.0s linear);
  @include animation-iteration-count(infinite);
}

````
