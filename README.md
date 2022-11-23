# About-Positions-in-css

Position in CSS
The position is one of the core properties of CSS like display or color. A better understanding of how you can position the elements on your HTML document can help you better visualize the end result.
The Position CSS property sets how an element is positioned in a document. The Top, Bottom, Right and Left properties determine the final location of positioned elements.
Here are some values of Position Property :
Absolute
Relative
Sticky
Fixed

Explanation:
1. Relative: If we add the top, bottom, right, and left values, it will move the position of the element which will be relative to its normal position based on the properties. The position is relative to the normal document flow.
<body>
    <div class="pos">1</div>
    <div class="pos1">2</div>
    <div class="pos">3</div>
   
</body>
    <style>
        body{
            display: flex;
        }
        .pos{
            height: 50px;
            width: 50px;
            background-color:#4DD637;
            color: black;
            border: 1px solid black;
        }
        .pos1{
            height: 50px;
            width: 50px;
            background-color:#03C6C7;
            position: relative;
            top: 50px;
        }

    </style>
2. Absolute: If we want to position the element to its parent and not to its relative position absolute property is used. This property is applied to parents. Its final position is determined by the values of the top, bottom, right, and left values.
<body>
    <div class="pos">1</div>
    <div class="pos1">2</div>
    <div class="pos">3</div>
   
</body>
 <style>
        body{
            display: flex;
        }
        .pos{
            height: 50px;
            width: 50px;
            background-color:#4DD637;
            color: black;
            border: 1px solid black;
        }
        .pos1{
            height: 50px;
            width: 50px;
            background-color:#03C6C7;
            border: 1px solid black;
            position: absolute;
            top: 50px;
            left: 50px;

        }

    </style>
3. Fixed: Fixed position places the element in a fixed place according to the viewport. Page Scrolling does not affect this position. Once fixed it will not change the position.
The best example of a fixed position element is a modal screen, chatbots, and sticky navigation.
4. Sticky: Sticky position is a combination of relative and fixed. It is relative until it crosses a specific point. But this position changes to fixed once it crossed a certain point basically a scroll point. If we scroll back again it will become a relative. we should provide top, bottom, right, and left values.
