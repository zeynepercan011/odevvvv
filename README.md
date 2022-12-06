# odevvvv

//dizinin en buyuk 2. elemanını döndüren fonksiyon

#include<stdio.h>


int ikincibuy(int matris[5])
{
    int max = matris[0];
    for (int i = 0; i<5; i++)
    {
        if (max < matris[i])
        {
            max = matris[i];
        }
    }

    int ikincibuy = matris[0];
    for (int i = 0; i <5; i++)
    {
        if (ikincibuy < matris[i] && matris[i] != max)
        {
            ikincibuy = matris[i];
        }
    }
    return ikincibuy;
}
