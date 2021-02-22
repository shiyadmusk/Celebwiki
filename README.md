# Celebwiki
@@ -511,9 +511,9 @@ def go_to_celeb(c):
                k = event.key
                isLetter = ord('a') <= k <= ord('z')
                if isLetter or k == ord('-') or k == ord(' ') or k == ord('\''):
                    ch = chr(k)
                    ch = event.unicode
                    if isShiftPressed and isLetter:
                        ch = chr(k - 32)
                        ch = ch.upper()
                    enteredName = enteredName + ch
                if len(enteredName) >= 1 and (k == K_BACKSPACE or k == K_DELETE):
                    enteredName = enteredName[0:-1]
