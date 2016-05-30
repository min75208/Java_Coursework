public class Project1 {
	
	static TextFileInput inFile;
	static String inFileName = "Words.txt";
	static int count = 0;
	static String[] Words, wordList, wordArray;
	
	public static void main(String[] args){
		
	    Project1GUI.initialize();
		wordList = readFile(inFileName);
		
		Project1GUI.output(wordList, "unsortedList", count);
		
		selectionSort(wordList);
		Project1GUI.output(wordList, "sortedList", count);
		
	}
	
	public static String[] readFile(String fileName){
		 
		Words = new String[100];
		inFile = new TextFileInput(fileName);
		String line;
		line = inFile.readLine();
		while(line != null){
			if(checkLetters(line)){
				Words[count]=line;
				count++;
			}
			line = inFile.readLine();
		}
		return Words;
	}
	
	public static boolean checkLetters( String checkWord){
		for (int i = 0; i < checkWord.length(); i++){
			 char findLetter = checkWord.charAt(i);
			 if (!Character.isLetter(findLetter)){
				 return false;
			 }
		}
		return true;
	}
	
	public static void selectionSort(String [] array){
		String temp;
		
		for(int i = 0; i < count - 1; i++){ 
	         int indexLowest = i;
	         for(int j = i + 1; j < count; j++){
	             if((array[j].compareTo(array[indexLowest])) < 0) 
	            	 indexLowest = j;
	         }
	         
	         if(array[indexLowest] != array[i]){
	            temp = array[indexLowest];
	            array[indexLowest] = array[i];
	            array[i] = temp;     
	         }
		}
	}
	
	
}
