#include <stdio.h>

int main() {
    char company[50];
    float budget;
    int visitors, customers;
    float conversionRate;

    printf("===== DIGITAL MARKETING PROGRAM =====\n");

    printf("Enter Company Name: ");
    scanf("%s", company);

    printf("Enter Marketing Budget (Rs): ");
    scanf("%f", &budget);

    printf("Enter Website Visitors: ");
    scanf("%d", &visitors);

    printf("Enter Number of Customers: ");
    scanf("%d", &customers);

    conversionRate = ((float)customers / visitors) * 100;

    printf("\n----- DIGITAL MARKETING REPORT -----\n");
    printf("Company Name      : %s\n", company);
    printf("Marketing Budget  : Rs %.2f\n", budget);
    printf("Website Visitors  : %d\n", visitors);
    printf("Customers         : %d\n", customers);
    printf("Conversion Rate   : %.2f%%\n", conversionRate);

    if (conversionRate >= 10)
        printf("Campaign Status   : Excellent\n");
    else if (conversionRate >= 5)
        printf("Campaign Status   : Good\n");
    else
        printf("Campaign Status   : Needs Improvement\n");

    return 0;
}
