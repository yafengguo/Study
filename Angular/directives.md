#Angualr Directives Properties/Method Summary
##restrict: String, 
restrict: EACM. 
  E=Element, <my-directive></my-directive>
  A=Attribute, <div my-directive="expression"></div>
  C=Class, <div class="my-directive:expression;"></div>
  N=Mark <--directive:my-directive expression-->
只有在申明的DOM类型中出现的tag扩展才会被关联当当前的directive上。



priority: Number, 
terminal: Boolean, 
template: String or Template Function: function(tElement, tAttrs) (...}, 
templateUrl: String, 
replace: Boolean or String, 
scope: Boolean or Object, 
transclude: Boolean, 
controller: String or function(scope, element, attrs, transclude, otherInjectables) { ... }, 
controllerAs: String, 
require: String, 
link: function(scope, iElement, iAttrs) { ... }, 
compile: // 返回一个对象或连接函数，如下所示：
            function(tElement, tAttrs, transclude) { 
                return { 
                        pre: function(scope, iElement, iAttrs, controller) { ... }, 
                        post: function(scope, iElement, iAttrs, controller) { ... } 
                    } 
// 或者 return function postLink(...) { ... }
