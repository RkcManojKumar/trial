function CheckDKRows3D(qid,qiddk, coltxt)  {
  if (!QuestionErrors()) {
    var codes = f(qid).domainValues()
    for (var i = 0; i<codes.length;i++) {
      var code = codes[i]
      if (!f(qid).item(code).toBoolean() && !f(qiddk).item(code).toBoolean()) {
        f('qErrNum_3').set(f('qTitle_'+coltxt).label());
        errorMsg(f('qErrors_36').label() + " " + f(qid).item(code).label()+": "+f('qErrors').item('1').label());
        f('qErrNum_3').set(null);
        break;
      }
      if (f(qid).item(code).toBoolean() && f(qiddk).item(code).toBoolean()) {
        f('qErrNum_3').set(f('qTitle_'+coltxt).label());
        errorMsg(f('qErrors_36').label() + " " +f(qid).item(code).label()+": "+f('qErrors').item('9').label()+f(qiddk).text()+f('qErrors').item('10').label());
        f('qErrNum_3').set(null);
        break;
      } 
    }
  }
}
