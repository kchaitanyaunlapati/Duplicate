# Duplicate
package comm.collection.classes;

import java.util.ArrayList;
import java.util.HashSet;

public class program {
	static ArrayList<String>removeDuplicates(ArrayList<String> list){
		
		//store unique item in result
		ArrayList<String> result=new ArrayList<>();
		
		//Record encountered Strings in HashSet.
		HashSet<String>set=new HashSet<>();
		
		// Loop over argument list.
		for(String item:list){
			if(!set.contains(item)){
				result.add(item);
				set.add(item);
				
			
			}
		}
	return result;
	
	}
	public static void main(String[] args) {
		ArrayList<String> list=new ArrayList<>();
		list.add("chaitanya");
		list.add("krishna");
		list.add("kumari");
		list.add("chaitanya");
		list.add("chaitanya");
		list.add("krishna");
		list.add("raadha");
		ArrayList<String> New =removeDuplicates(list);
		for (String element : New) {
		    System.out.println(element);
		}
		
	}
	

}
