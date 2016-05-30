import javax.swing.JOptionPane;


public class Project0 {
	
		public static void main(String[] args) {

		   		String inputWord = "";
		   								
				while( !inputWord.equalsIgnoreCase("Stop")){
										
					inputWord = JOptionPane.showInputDialog(null, "Please enter a sentence:");
					
					int e_counter = 0, E_counter = 0;
					
					for( int i =0; i<inputWord.length(); i++){
							
						if(inputWord.charAt(i) == 'e')
							e_counter++;
						if(inputWord.charAt(i) == 'E')
							E_counter++;
					}
					
					JOptionPane.showMessageDialog(null, "Number of lower case e's: "+ e_counter+"\nNumber of upper case e's: "+ E_counter);
				}
				
		}//main
		
}
