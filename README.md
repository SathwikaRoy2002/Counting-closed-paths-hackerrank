int closedPaths(int number) {
    int sum = 0;
        while(number!=0) {
            int ch = number%10;
            if(ch==0 || ch ==4 || ch==6 || ch==9) {
                sum = sum + 1;
            }
            if(ch==8) {
                sum = sum +2;
            }
        number = number/10;
    }
    return sum;
}
