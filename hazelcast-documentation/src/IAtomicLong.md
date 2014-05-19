

## IAtomicLong


Hazelcast IAtomicLong is the distributed implementation of  `java.util.concurrent.atomic.AtomicLong`. It offers most of AtomicLong's operations such as `get`, `set`, `getAndSet`, `compareAndSet` and `incrementAndGet`. Since IAtomicLong is a distributed implementation, these operations involve remote calls and hence their performances differ from that of AtomicLong.


	IAtomicLong counter = hz.getAtomicLong("counter");
		if (k % 500000 == 0){ System.out.println("At: "+k);
	}
```


	@Override
		return input +2;
}




```java
public class Member {
		IAtomicLong atomicLong = hz.getAtomicLong("counter");
		System.out.println("apply.result:" + result); 		
		System.out.println("apply.value:" + atomicLong.get());
		System.out.println("alter.value:"+atomicLong.get());
		System.out.println("alterAndGet.result:" + result); 		
		System.out.println("alterAndGet.value:"+atomicLong.get());
		System.out.println("getAndAlter.result:"+result); 		
		System.out.println("getAndAlter.value:"+atomicLong.get());
	}
```