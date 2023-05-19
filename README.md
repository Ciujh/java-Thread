# java-Thread

public class Main
{
    public static class ThreadBasica extends Thread{
        public ThreadBasica(String nome ){
            super(nome);
        }
        @Override
        public void run(){
         for (int i=0;i<10;i++){
             System.out.println(i+""+getName());
         }
        }
    }
	public static void main(String[] args) {
		System.out.println("Hello World");
	   new ThreadBasica ("").start(); 
	}
}

