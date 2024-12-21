# -RSA-IBE-
测试案例
模数这块：
    bit_length = 0  # RSA模数
    if λ == 128:
        bit_length = 512
    elif λ == 192:
        bit_length = 1536
    elif λ == 256:
        bit_length = 2024
因为设备有限，我都除以2，真实情况要乘回去2
运行时间很长
解密那块代码我就简化了，实际上要求r^2 mod N,然后确定是s1还是s2
