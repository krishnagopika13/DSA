package advanced;
import java.util.*;

public class BinaryTree {
	static Scanner sc;
	public static void main(String[] args) {
		BinaryTree b = new BinaryTree();
		node root = b.createtree();
		b.preorder(root);
		System.out.println();
		b.inorder(root);
		System.out.println();
		System.out.println(b.height(root));
		System.out.println(b.size(root));
	
	}
	public node createtree() {
		System.out.println("enter the data");
		sc = new Scanner(System.in);
		int data;
		try {
		   data=sc.nextInt();

		}
		catch(Exception e) {
		   return null;

		}
		node root = new node(data);
		System.out.println("left node for "+data);
		root.left=createtree();
		System.out.println("right node for "+data);
		root.right=createtree();
		return root;
	}
	public void preorder(node root){
		node n = root;
		if(n==null)
		{
		   return;
		}
		System.out.print(n.data+" ");
		preorder(n.left);
		preorder(n.right);
		
	}
	public void inorder(node root) {
		
			node n = root;
			if(n==null)
			{
				return;
			}
			inorder(n.left);
			System.out.print(n.data+ " ");
			inorder(n.right);

			
	}
	
	
	





public int height(node root) {
	node n=root;
	if(n==null)
	{
		return 0;
	}
	return Math.max(height(n.left), height(n.right))+1;
 }
	
public int size(node root) {
	node n=root;
	if(n==null) {
		return 0;
	}
	return size(n.left)+ size(n.right)+1;
}

}


class node{
	node left;
	node right;
	int data;
	node(int data){
		this.data= data;
	}	

}
