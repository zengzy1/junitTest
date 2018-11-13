/**
 * 
 */
package www.action;

import org.junit.Test;

public class TestAction {
	
	/**
	 * 打印1-100的数字和转义单词
	 * @author zengzy
	 * @since jdk1.8
	 * @date 2018-11-12
	 * @return 
	 * */
	@Test
	public void printNumbers(){
		int number = 100; //赋值最大值100
		
		// for循环遍历数值,并打印
		for(int i=1;i<=number;i++){
			if(i % 15 == 0){ //能被三和五整除的数字, 相当于15的倍数(包括15)
				System.out.println("FizzBuzz");
				continue;
			} else if(i % 3 == 0){ //能被三整除的数字(包含3)
				System.out.println("Fizz");
				continue;
			} else if(i % 5 == 0){//能被五整除的数字(包含5)
				System.out.println("Buzz");
				continue;
			};
			
			System.out.println(i);
			
		}
	}
}
