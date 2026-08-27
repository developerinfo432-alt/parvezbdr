# User Input
print(f"{CYAN}[+] Initializing DarkNet Proxies...{RESET}")
time.sleep(1)
print(f"{GREEN}[OK] 12 Proxy Nodes Connected Successfully.{RESET}\n")

target_num = input(f"{YELLOW}[?] Enter Victim's Phone Number/ID: {RESET}")

if not target_num:
    print(f"{RED}[!] Error: Target field cannot be empty!{RESET}")
    return

print(f"\n{CYAN}[*] Targeting Account: {WHITE}{target_num}{RESET}")
slow_print(f"{CYAN}[*] Fetching Profile ID & Access Tokens...{RESET}", 0.02)
fast_dots(4)

# Fake Hack Steps
print(f"{GREEN}[✓] Account Found! Payload Injected Successfully.{RESET}")
time.sleep(1)

print(f"\n{PURPLE}[>] Starting Automated Dictionary Attack...{RESET}")
time.sleep(1)

matrix_effect(4)

passwords_list = [
    "pass123456", "bangladesh123", "secret_pass", "fb_user_99", 
    "iloveyou2026", "admin_portal_77", "qwertyuiop", "dragon_king"
]

for pwd in passwords_list:
    status = f"{RED}[FAILED]{RESET}"
    print(f"{WHITE}[+] Testing Hash: {pwd:<20} Status: {status}")
    time.sleep(random.uniform(0.15, 0.4))
    
print(f"\n{YELLOW}[!] Bypassing 2FA Authentication Guard...{RESET}")
fast_dots(5)

fake_cracked_pass = f"FB_{target_num[-4:] if len(target_num)>=4 else '99'}_" + str(random.randint(1000, 9999))

print(f"\n{GREEN}=================================================={RESET}")
print(f"{GREEN}[★] EXPLOIT SUCCESSFUL! ACCOUNT COMPROMISED{RESET}")
print(f"{WHITE}Target    : {target_num}{RESET}")
print(f"{WHITE}Password  : {YELLOW}{fake_cracked_pass}{RESET}")
print(f"{WHITE}Auth Token: {PURPLE}EAAAE{random.randint(100000,999999)}ZX901A{RESET}")
print(f"{GREEN}=================================================={RESET}\n")
