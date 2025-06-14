WIZnet-PICO-C　HTTP ServerのDHCP用のプログラムになります。
[https://github.com/WIZnet-ioNIC/WIZnet-PICO-C](https://github.com/WIZnet-ioNIC/WIZnet-PICO-C/tree/main/examples/http/server)

以下2ファイルを書き換えます。
CMakeLists.txt
wizchip_http_server.c

以下のコメントアウトを外すことでDHCPになります。
```
//DHCP
/* 
    wizchip_dhcp_init();

    while (1)
    {
        if (DHCP_IP_LEASED == DHCP_run())
            break;
    }
*/
  
```
