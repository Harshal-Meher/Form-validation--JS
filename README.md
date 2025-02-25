1. Form Validation -Logic  : - split method use not allow @@ and not use @ invalid
 
       if(email.length === 0) {
            alert("Please enter email");
            document.getElementById('email').focus();
            return false;
        } else {
            let atCount = email.split('@').length - 1;
           -----------------------------------------------
            if(atCount !== 1 || email.includes()){
                alert('Not Valid');
                return false;
            }
        }
 
