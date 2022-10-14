#! /bin/bash
for i in {1..100}
do
    if [ $i -eq 100 ];
    then
	echo "user$i.public	IN	CNAME	fw.sabang.net." >> sabang.net
    elif [ $i -lt 10 ];
    then
	echo "user00$i.public	IN	CNAME	fw.sabang.net." >> sabang.net
    else
	echo "user0$i.public	IN	CNAME	fw.sabang.net." >> sabang.net
    fi
done
