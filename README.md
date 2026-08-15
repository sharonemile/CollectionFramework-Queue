package com.sharon;

	import java.util.LinkedList;
	import java.util.Queue;

	public class StudentSupportQueue {
		public static void main(String[] args) {
			Queue<String> studentQueue = new LinkedList<>();

			studentQueue.add("Domnic");
			studentQueue.add("Therasa");
			studentQueue.add("Angel");
			System.out.println("Enqueued 3 students.");

			String firstStudent = studentQueue.peek();
			System.out.println("First student in line: " + firstStudent);

			System.out.println("\nProcessing students from the queue:");
        
			while (!studentQueue.isEmpty()) {
				String removedStudent = studentQueue.poll(); 
				System.out.println("Processed student: " + removedStudent);
        }
    }
}

OUTPUT:

  Enqueued 3 students.
  
  First student in line: Domnic

  Processing students from the queue:

  Processed student: Domnic
  
  Processed student: Therasa
  
  Processed student: Angel
