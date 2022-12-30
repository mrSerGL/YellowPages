
; ===== HTML =====

<div class="container">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
</div>

; ===css===

.container {

     width: 480px;
     margin: auto;
     padding: 15px;
    
    display: flex;
    justify-content: space-between;
    align-items: center;
   
}

.box {
   width: 130px;
   min-height: 75px;
    
    
   display: flex;
   justify-content: center;
   align-items: center;
   
}

; ===== CSS =====

body {
  font-size: 20px;
    box-sizing: border-box;
}

;   2 * 15 - это размер, 
;   который box-sizing: border-box 
;   отнял у width и height

;   ширина container 480  - (2 * 15)
;   или 3 раза по 160 - (2 * 15)  

.container {

  width: 480px;
  margin: auto;
  padding: 15px;
  
display: flex;

flex-direction: row | row-reverse | column | column-reverse;   
# устанавливает направление главной оси, определяя направление элементов в контейнере.
   
justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly
# элементы на главной оси

        align-items:     stretch | flex-start | flex-end | center | baseline
        # элементы вдоль поперечной оси

flex-wrap:       nowrap | wrap | wrap-reverse
# перенос элементов разрешить

gap: xxpx;
# комбинирует в себе значение свойств row-gap и column-gap, которые позволяют отдельно указать размеры зазоров между строками и столбцами сетки. Используйте gap когда зазоры одинаковые, в противном случае подойдут row-gap и column-gap

        align-content:   flex-start | flex-end | center | space-between |    space-around |         space-evenly | stretch
        # Управляет выравниванием всех строк многострочного контейнера вдоль поперечной оси, если         есть свободное место. Аналогично тому, как justify-content выравнивает элементы в каждой         строке. Это свойство не действует, когда есть только одна строка элементов или в контейнере         нет свободного места по вертикали (явно не задана высота больше чем контент).

}

.box {
  width: 130px;
  min-height: 75px;
    
    display: inline-flex;

    justify-content: center;
    align-items: center;
}

; ===============================================================================





===== Свойства родительских элементов (flex-container) =====


# display

     .container {
       display: flex; /* или inline-flex */ }

       Создаёт flex-контейнер, блочный или строчно-блочный, в зависимости от заданного значения, и устанавливает flex-контекст для всех детей (не потомков) контейнера, превращая их во flex-элементы.

#flex-direction     

     Устанавливает направление главной оси и определяет направление flex элементов 

     .container {
     flex-direction: row | row-reverse | column | column-reverse;}

     - row (стандартное положение) — слева направо.
     - row-reverse — элементы располагаются справа налево.
     - column — тоже самое, что и row, только сверху вниз.
     - column-reverse — тоже самое, что и row-reverse, но снизу вверх.

#flex-wrap      

     возможность элементам переходить на другую строку

     .container{
       flex-wrap: nowrap | wrap | wrap-reverse;
     }

     nowrap — это значение по-дефолту, при котором все flex элементы будут выстраиваться в одну линию.
     wrap — flex элементы будут переноситься на несколько строк, от верха к низу.
     wrap-reverse — flex элементы будут переноситься на несколько строк снизу вверх.

#flex-flow        сокращение flex-direction и flex-wrap свойств (применяется для родительского flex контейнера)


     flex-flow: <'flex-direction'> || <'flex-wrap'>

#justify-content  

     определяет выравнивание вдоль главной оси

     .container {
            justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
     }

     flex-start — дефолтное состояние, при котором элементы расставляются от начала строки.
     flex-end — состояние, в котором элементы размещены с конца строки.
     center — элементы центрированы вдоль строки.
     space-between — элементы равномерно распределены по строке, первый элемент находится вначале строки, последний в конце.
     space-around — элементы равномерно распределены по строке с равным местом вокруг них. Учтите, что визуально пробелы не равномерны, так как все элементы имеют 
                    одинаковые пробелы с двух сторон. Первый элемент получит одну единицу свободного места от границы контейнера, но получит две единицы свободного 
                    места от следующего элемента, так как у него тоже есть одна единица свободного места с каждой из сторон.
     space-evenly — элементы распределены таким образом, что свободное пространство между любыми двумя элементами равномерно, как и место до границы края контейнера.

#align-items

     определяет как flex элементы будут располагаться вдоль поперечной оси на заданной строке

     .container {
       align-items: stretch | flex-start | flex-end | center | baseline;
     }

     flex-start — всё размещается с начала поперечной оси
     flex-end — все элементы размещаются с конца поперечной оси
     center — элементы центрируются по поперечной оси
     baseline — элементы выравниваются по базовой линии
     stretch — это дефолтное состояние, при котором элементы заполяют контейнер, с учетом min-width и max-width.

#align-content

     выравнивает и распределяет строки контейнера в поперечной оси

     .container {
       align-content: flex-start | flex-end | center | space-between | space-around | stretch;
     }
     flex-start — строки расположены от начала контейнера.
     flex-end — строки расположены от конца контейнера.
     center — строки расположены от центра контейнера.
     space-between — строки равномерно распределены, первая строка находится вначале контейнера, тогда как последняя находится в конце.
     space-around — строки равномерно распределены с равным местом вокруг каждой строки.
     stretch — стандартное состояние, при котором строки растягиваются на вся оставшееся место.



===== Свойства дочерних элементов =====


#Order

     контролирует порядок в котором элементы могут располагаться.

     .item {
       order: <любое целое число>; /* дефолтное 0 */
     }


#flex-grow

     определяет способность flex элемента становится больше

     .item {
       flex-grow: <число>; /* дефолтное 0 */
     }

#flex-shrink

     определяет способность flex элемента сокращаться

     .item {
       flex-shrink: <число>; /* дефолтное 1 */
     }

#flex-basis
     определяет стандартный размер элемента, перед тем как оставшееся место будет распределено

     .item {
       flex-basis: <длина> | auto; /* дефолтное auto */
     }

#flex

     Это сокращение для flex-grow, flex-shrink и flex-basis

     .item {
       flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
     }

#align-self

     позволяет стандартному выравниванию (или если точно align-items) элементов, быть перезаписанному для определенного flex элемента.

     .item {
       align-self: auto | flex-start | flex-end | center | baseline | stretch;
     }
