```java
        byte myAge = 30; // 1 byte [-128, 127]
        short years = 20000; // 2 bytes [-32k, 32k]
        int universe = 300000; // 4 bytes [-2B, 2B]
        long viewsCount = 3_123_456_789L; // 8 bytes _ to seperate every three digits
        
        float price = 10.99F; // 4 bytes
        double people = 4; // 8 bytes

        char letter = 'A'; // 2 bytes each
        
        boolean isEligible = true; // 1 byte
   
        Date now = new Date();
        now.getTime();
        System.out.println(now);

        Point point1 = new Point(1, 1);
        String message = "Hello there"; // strings are ref types in Java
        System.out.println(message.endsWith("d"));
`