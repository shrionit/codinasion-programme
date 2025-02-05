---
title: Volume of Sphere
description: Write a program to compute the volume of a Sphere
tags:
  - python
  - java
contributors:
  - aashish-khub
  - zhixuanevelynwu
---

## Write a program to compute the volume of a Sphere

Volume of a sphere = radius \* radius \* radius \* 4/3 \* π

```
Radius : 8

Volume : 2144.66
```

---

<CodeBlock>

```python
import math

# Get radius from user
enter_radius = int(input('Radius : '))

# Calculate volume
volume = enter_radius * enter_radius * enter_radius * 4/3 * math.pi

# Print result
print("\nVolume : {:0.2f}".format((volume)))
```

```java
import java.util.Scanner;

public class VolumeOfSphere {
	private static double computeSphereVolume(double r) {
		return r * r * r * 4 / 3 * Math.PI;
	}

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.print("Radius : ");
		double r = sc.nextDouble();
		double vol = computeSphereVolume(r);
		System.out.printf("\nVolume : %.2f\n", vol);
		sc.close();
	}
}
```

</CodeBlock>
