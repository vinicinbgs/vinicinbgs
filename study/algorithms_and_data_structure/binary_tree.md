### What's binary tree?
Is a data structure in which each node has at most two children, which are referred to as the left children and right children. <br>
Each vertice can be 0, 1 or 2 number of childrens
```
            ______7_______             |   1 depth
           /              \
        __3__           ___11___       |   2 depth
       /     \         /        \
      1       5       9         _13    |   3 depth
     / \     / \     / \       /   
    0   2   4   6   8   10    12       |   4 depth
```

- (LEAF) a leaf is a node that doesn't have any children
- (PATH) the path is nodes that are interconnected and the length of the path is the number of nodes or number of edges
- (DEPTH) number of edges from the root node to the leaf node of the tree is called as the Depth of the Tree


Java Solution to mount a binary tree and get maximum height
```java
import java.util.*;
import java.io.*;

class Node {
    Node left;
    Node right;
    int data;
    
    Node(int data) {
        this.data = data;
        left = null;
        right = null;
    }
}

class Solution {
    public static int height(Node root) {
          if(root == null) return -1;
          
        int leftHeight = 0, rightHeight = 0;
        
        if(root.left != null) leftHeight = height(root.left) + 1;
        if(root.right != null) rightHeight = height(root.right) + 1;
        
        return Math.max(leftHeight, rightHeight);
    }

    public static Node insert(Node root, int data) {
        if(root == null) {
            return new Node(data);
        }
    
       Node cur;
       if(data <= root.data) {
            cur = insert(root.left, data);
            root.left = cur;
        } else {
            cur = insert(root.right, data);
            root.right = cur;
        }
        
        return root;
}

public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        Node root = null;
        
        int data = scan.nextInt();
        
        while(data-- > 0) {
            root = insert(root, scan.nextInt());
        }
        
        scan.close();
        
        int height = height(root);
        System.out.println(height);
    }    
}

```
