
List_remove

-checks if first and last nodes are empty
-checks if node is NULL
-if node is first and last it is the only node so it turns both of them to NULL
-else if node is first make the first node the next node then make prev node NULL which is what the new node is pointing to
-else if node is last make the prev node the last and then make the node next which was the old last node NULL
-else if in middle create two structs one called after and one called before, Make a temp struct called after with the pointer to the next node, and make temp struct called before with the pointer prev (thus begins the breaking of the nodes connections). Take the new struct after and assign the previous pointer to the before struct, and take the before struct's next pointer and set it to after. This establishes a new connection to before and after. 
-decrement the count to account for the removal of the node
-make a variable called result equal to that nodes value
-free that nodes result that nodes result from memory
n two cases it looks at the first or last node and then looks at the next or prev node and makes those the first or last and then makes the original nodes NULL. If its in the middle it assigns the nodes adjacent as before and after and then takes the pointers and connects them to their next or prev nodes, thus removing the node in question

List_pop

-take off the last value
-takes a list value
-declare list a pointer to the pointer last in the list struct type ListNode struct
-if node != NULL do List_remove(list, node) else NULL

List_push

-make new last node
-Takes list and value
-declare node a pointer to allocated memory size of listnode type struct listnode
-check_mem for node
-assign value to the value in the struct
-If the list last is NULL if there are no items in the chain
make the node the first and last (the only)
-else look for the last node and point to the current node
make the current node point prev to the old last node
and finally make the node the last in the list
-increment the count

List_unshift

-make first node
-take list and a value
-decalre node a pointer to allocated memory the size of listnode
type Listnode struct
-check memory
-assign value to the value passed
-if the first value is null make the node the only node
-else take the node next pointer and point to the first item in
the list
-take the old first node and assign previous to the new node
-make the new node the first in the list struct

List_shift

-
-Takes a pointer to the list struct list struct
-declare node a pointer to the first node in the list type
listnode struct
-if node != NULL remove that node else NULL



















