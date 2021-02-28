```java

//demo.txt
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus a diam placerat, rutrum lorem in, auctor mauris. Donec et sapien lectus. Aliquam erat volutpat. Donec nec vehicula diam. In finibus fermentum eros, vel rhoncus augue tincidunt a. Cras a feugiat augue. Fusce blandit at neque sed auctor. Vestibulum eget iaculis nunc, eget auctor mauris. Donec sit amet vestibulum dolor.

Mauris mollis eleifend quam id imperdiet. Nulla ac odio nunc. Praesent nec egestas lacus. Maecenas accumsan, velit non accumsan dictum, ante lectus venenatis ante, vitae placerat erat est sodales tellus. Cras sit amet arcu et nisl finibus efficitur vitae ac nisl. Aliquam vel lacus lorem. Praesent rutrum pellentesque lectus id tempor. Vivamus vulputate arcu eget tincidunt luctus. Fusce sit amet elit arcu. Nullam sodales imperdiet nibh, efficitur tristique sapien laoreet et. Phasellus nec elit ac sapien cursus dapibus. Phasellus rutrum nunc mi, a accumsan mi condimentum vel. Cras malesuada tempor purus sed molestie.

import java.io.*;

public class question9 extends Exception {
    private static final long serialVersionUID = 1L;

    public static void validate(File f, int k) {
        long a = f.length();
        System.out.println(a);
        if(a <= k)
            throw new ArithmeticException("Lower than " + k);
    }
    public static void main(String[] args){
        File f = new File("demo.txt");
        validate(f, 2500);
    }
}


```
