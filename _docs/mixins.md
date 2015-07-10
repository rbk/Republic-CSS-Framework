**box-shadow() mixin**
```scss
// Input
.element {
	@include box-shadow(0, 1px, 1px, rgba(0, 0, 0, 0.075));
}

// Output
.element {
	-webkit-box-shadow: 0, 1px, 1px, rgba(0, 0, 0, 0.075);
	-moz-box-shadow: 0, 1px, 1px, rgba(0, 0, 0, 0.075);
	box-shadow: 0, 1px, 1px, rgba(0, 0, 0, 0.075);
}
```

**opacity mixin**
```scss
// Input
.element {
	@include opacity(0.9);
}

// Output
.element {
	-ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=" 90 ")";
    filter: alpha(opacity= 90 );
    -moz-opacity: 0.9;
    -khtml-opacity: 0.9;
    opacity: 0.9;
}
```

**transform mixin**
```scss
// Input
.element {
	@include transform(rotate(42deg));
}

// Output
.element {
	-webkit-transform: rotate(42deg);
	-moz-transform: rotate(42deg);
	-ms-transform: rotate(42deg);
	transform: rotate(42deg);
}
```

**keyframe mixin**
```scss
// Input
@include keyframe(color) { 
	0% { 
		color: #fff; 
	} 
	100% { 
		color: #000; 
	} 
}

// Output
@-webkit-keyframes color {
	0% { 
		color: #fff; 
	} 
	100% { 
		color: #000; 
	} 
}
@-moz-keyframes color {
	0% { 
		color: #fff; 
	} 
	100% { 
		color: #000; 
	} 
}
@-ms-keyframes color {
	0% { 
		color: #fff; 
	} 
	100% { 
		color: #000; 
	} 
}
@keyframes color {
	0% { 
		color: #fff; 
	} 
	100% { 
		color: #000; 
	} 
} 


```