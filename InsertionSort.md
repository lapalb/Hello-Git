#function [ k ] = is( a,n )
%This is insertion sort routine and it gives number of comparision done.
k=0;
for i=2:n
    key=a(i);
    j=i-1;
    while(j>0 && a(j)>key)
        k=k+1;
        a(j+1)=a(j);
        j=j-1;
    end
    a(j+1)=key;
end
end

