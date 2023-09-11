# Goldman Sachs Forage Job Simulation

## Table of Contents

- [Memo](#memo)
- [Requirements](#requirements)
- [Usage](#usage)
- [Results](#results)
- [Author](#author)

**Subject**: Assessment of Password Policy and Recommendations for Improvement

## Memo

```txt
Dear Sir/Ma'am,

I trust this message finds you well. Allow me to extend my gratitude for your attention to the matter at hand. My objective in reaching out to you is to provide a comprehensive assessment of our current password policy, along with a series of recommendations aimed at enhancing our data security practices.

Upon a thorough examination of the leaked password hashes, it has come to my attention that our password policy is in need of significant improvement. The vulnerabilities discovered primarily stem from the utilization of the Message Digest 5 (MD5) hash function, a cryptographic algorithm that is known for its vulnerability to collisions. This made it susceptible to exploitation, as evidenced by the relatively straightforward cracking process using tools such as Hashcat.com in conjunction with readily available wordlists like 'rockyou.txt' via terminal and web browsers. In light of these findings, I would strongly recommend transitioning to a more robust password encryption mechanism, such as the Secure Hash Algorithm (SHA), to fortify our data security measures.

The analysis of the compromised passwords revealed the following key shortcomings in our current password policy:

1. **Inadequate Minimum Password Length:** Our current policy stipulates a minimum password length of 6 characters, which falls short of industry best practices.
2. **Lack of Specific Password Creation Requirements:** Our policy does not provide clear guidelines on password creation, permitting users to employ any combination of words and letters, which is inherently insecure.

In light of these findings, I offer the following recommendations for the enhancement of our password policy:

1. **Stringent Password Complexity:** Implement more stringent requirements for password complexity, including the use of special characters, both uppercase and lowercase letters, and numbers. These elements significantly bolster the strength of passwords.
2. **Minimum Password Length:** Raise the minimum password length to at least 8 characters. Longer passwords are inherently more secure, and 8 characters should serve as a baseline.
3. **Password Reuse Prevention:** Discourage password reuse across different accounts to mitigate the risks associated with compromised credentials.
4. **Prohibition of Personal Information:** Prohibit the inclusion of personally identifiable information, such as usernames, actual names, dates of birth, or any other easily accessible personal data, in passwords.
5. **User Education:** Provide comprehensive training and awareness campaigns to educate users on the importance of adhering to these password policies and best practices to safeguard their accounts and sensitive information.

By implementing these recommendations, we can significantly enhance the security of our digital assets and reduce the risk of unauthorized access. I believe that a proactive approach to strengthening our password policy is crucial in safeguarding our organization against potential security threats.

I appreciate your consideration of these findings and recommendations, and I look forward to collaborating with you to further bolster our security measures. Should you require any additional information or clarification, please do not hesitate to reach out.

Sincerely,

Mantresh Kumar
B.Tech Computer Science and Engineering
```

## Requirements

- [Hashcat](https://hashcat.net/hashcat/)
- [Rockyou.txt](https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt)

## Usage

```bash
hashcat -m 0 -a 0 -o decrypted.txt hashes.txt rockyou.txt # to crack pass
hashcat -m 0 -a 0 -o decrypted.txt hashes.txt rockyou.txt --show # to see it again after 1st time decryption
```

## Results

```sh
Security Algorithms used(listed below): 

experthead:e10adc3949ba59abbe56e057f20f883e – MD5
interestec:25f9e794323b453885f5181f1b624d0b – MD5
ortspoon:d8578edf8458ce06fbc5bb76a58c5ca4 –MD5
reallychel:5f4dcc3b5aa765d61d8327deb882cf99 –MD5
simmson56:96e79218965eb72c92a549dd5a330112 – MD5
bookma:25d55ad283aa400af464c76d713c07ad – MD5 
popularkiya7:e99a18c428cb38d5f260853678922e03 – MD5
eatingcake1994:fcea920f7412b5da7be0cf42b8c93759 – MD5 
heroanhart:7c6a180b36896a0a8c02787eeafb0e4c – MD5
edi_tesla89:6c569aabbf7775ef8fc570e228c16b98 – MD5
liveltekah:3f230640b78d7e71ac5514e57935eb69 – MD5
blikimore:917eb5e9d6d6bca820922a0c6f7cc28b – MD5
johnwick007:f6a0cb102c62879d397b12b62c092c06 – MD5
flamesbria2001:9b3b269ad0a208090309f091b3aba9db – MD5
oranolio:16ced47d3fc931483e24933665cded6d - MD5
spuffyffet:1f5c5683982d7c3814d4d9e6d749b21e - MD5
moodie:8d763385e0476ae208f21bc63956f748 - MD5
nabox:defebde7b6ab6f24d5824682a16c3ae4 - MD5
bandalls:bdda5f03128bcbdfa78d8934529048cf - MD5

Cracked Passwords(listed below):

experthead:e10adc3949ba59abbe56e057f20f883e - 123456
interestec:25f9e794323b453885f5181f1b624d0b - 123456789
ortspoon:d8578edf8458ce06fbc5bb76a58c5ca4 - qwerty
reallychel:5f4dcc3b5aa765d61d8327deb882cf99 - password
simmson56:96e79218965eb72c92a549dd5a330112 - 111111
bookma:25d55ad283aa400af464c76d713c07ad - 12345678
popularkiya7:e99a18c428cb38d5f260853678922e03 - abc123
eatingcake1994:fcea920f7412b5da7be0cf42b8c93759 - 1234567
heroanhart:7c6a180b36896a0a8c02787eeafb0e4c - password1
edi_tesla89:6c569aabbf7775ef8fc570e228c16b98 - password!
liveltekah:3f230640b78d7e71ac5514e57935eb69 - qazxsw
blikimore:917eb5e9d6d6bca820922a0c6f7cc28b - Pa$$word1
johnwick007:f6a0cb102c62879d397b12b62c092c06 - bluered
```

## Author

- [Mantresh Khurana](https://github.com/mantreshkhurana)
