unit Unit2;

{$mode objfpc}{$H+}

interface

uses
  Windows, Messages, SysUtils, Variants, Classes, Graphics, Controls, Forms,
  Dialogs, Menus, StdCtrls, ExtCtrls, Buttons, Math,
  ComCtrls,clipbrd;

type

  { TForm2 }

  TForm2 = class(TForm)
    But20: TButton;
    But21: TButton;
    But22: TButton;
    Button1: TButton;
    Button10: TButton;
    Button11: TButton;
    Button12: TButton;
    Button13: TButton;
    Button14: TButton;
    Button15: TButton;
    Button16: TButton;
    Button0: TButton;
    Button2: TButton;
    Button3: TButton;
    Button4: TButton;
    Button5: TButton;
    Button6: TButton;
    Button7: TButton;
    Button8: TButton;
    Button9: TButton;
    Edit1: TEdit;
    Edit2: TEdit;
    RadioButton1: TRadioButton;
    RadioButton2: TRadioButton;
    RadioButton3: TRadioButton;
    RadioButton4: TRadioButton;
    procedure But20Click(Sender: TObject);
    procedure But21Click(Sender: TObject);
    procedure But22Click(Sender: TObject);
    procedure Button16Click(Sender: TObject);
    procedure Button9Click(Sender: TObject);
    procedure ClickBut(Sender: TObject);
    procedure ClickZnak(Sender: TObject);
    procedure Edit1Change(Sender: TObject);
    procedure Edit2Change(Sender: TObject);
    procedure FormCreate(Sender: TObject);
    procedure RadioButton1Change(Sender: TObject);
    procedure RadioButton2Change(Sender: TObject);
    procedure RadioButton3Change(Sender: TObject);
    procedure RadioButton4Change(Sender: TObject);
  private
    { private declarations }
  public
    { public declarations }
  end;

var
  Form2: TForm2; SS:extended;
  SS1:integer;
  const
  digit: string[36] = '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ';

implementation
uses unit1;

{$R *.lfm}
//dec v luboi ss
function FromDec(n, r: longint): string;
var
  s: string;
begin
  s := '';
  repeat
    s := digit[(n mod r) + 1] + s;
    n := n div r;
  until n = 0;
  FromDec := s;
end;

{ TForm2 }

procedure TForm2.ClickBut(Sender: TObject);
begin
  Edit1.Text:=Edit1.Text + ( Sender as TButton).Caption;

end;

procedure TForm2.Button9Click(Sender: TObject);
begin

end;

procedure TForm2.Button16Click(Sender: TObject);
begin
   Form2.hide;
   Form1.show;
end;

procedure TForm2.But22Click(Sender: TObject);
var
 str : String;
begin
  str := Edit1.Text;
  if str <> '' then
   Delete(str, Length(str),1);
  Edit1.Text:= str;
end;

procedure TForm2.But21Click(Sender: TObject);
begin
  Edit1.Clear;
end;

procedure TForm2.But20Click(Sender: TObject);
begin
  Edit1.Clear;
  a:=0;
  b:=0;
  c:=0;
end;

procedure TForm2.ClickZnak(Sender: TObject);
begin
  a := StrToFloat(Edit1.Text);
  Edit1.Clear;

  znak :=(Sender as TButton).Caption;
end;

procedure TForm2.Edit1Change(Sender: TObject);
begin

end;

procedure TForm2.Edit2Change(Sender: TObject);
begin

end;

procedure TForm2.FormCreate(Sender: TObject);
begin
    SS1:=10;
  Edit2.Text:=floattostr(SS1);
    Button10.Enabled:=false;
  Button11.Enabled:=false;
  Button12.Enabled:=false;
  Button13.Enabled:=false;
  Button14.Enabled:=false;
  Button15.Enabled:=false;
  end;

procedure TForm2.RadioButton2Change(Sender: TObject);
var s: string;
    n,m,k: integer;
begin
  if SS1=16 then
begin
  k:=0;
  s:=Edit1.Text;
  n:=Length(s);
  for m:=1 to n do begin
    k:=k*16;
    case s[m] of
      '0': k:=k+0;
      '1': k:=k+1;
      '2': k:=k+2;
      '3': k:=k+3;
      '4': k:=k+4;
      '5': k:=k+5;
      '6': k:=k+6;
      '7': k:=k+7;
      '8': k:=k+8;
      '9': k:=k+9;
      'A': k:=k+10;
      'B': k:=k+11;
      'C': k:=k+12;
      'D': k:=k+13;
      'E': k:=k+14;
      'F': k:=k+15;
    end;
  end;
  Edit1.Text:=IntToStr(k);
end
else if SS1=8 then
  begin
    k:=0;
    s:=Edit1.Text;
    n:=Length(s);
    for m:=1 to n do begin
      k:=k*8;
      case s[m] of
        '0': k:=k+0;
        '1': k:=k+1;
        '2': k:=k+2;
        '3': k:=k+3;
        '4': k:=k+4;
        '5': k:=k+5;
        '6': k:=k+6;
        '7': k:=k+7;
      end;
    end;
    Edit1.Text:=IntToStr(k);
  end
else if SS1=2 then
    begin
      k:=0;
      s:=Edit1.Text;
      n:=Length(s);
      for m:=1 to n do begin
        k:=k*2;
        case s[m] of
          '0': k:=k+0;
          '1': k:=k+1;
        end;
      end;
      Edit1.Text:=IntToStr(k);
end;
 SS1:=10;
  Edit2.Text:=inttostr(SS1);
  Button1.Enabled:=true;
  Button2.Enabled:=true;
  Button3.Enabled:=true;
  Button4.Enabled:=true;
  Button5.Enabled:=true;
  Button6.Enabled:=true;
  Button7.Enabled:=true;
  Button8.Enabled:=true;
  Button9.Enabled:=true;
  Button0.Enabled:=true;
  Button10.Enabled:=false;
  Button11.Enabled:=false;
  Button12.Enabled:=false;
  Button13.Enabled:=false;
  Button14.Enabled:=false;
  Button15.Enabled:=false;
  end;


 procedure TForm2.RadioButton1Change(Sender: TObject);
 var s: string;
     n,m,k: integer;
 begin
  if SS1=10 then
    begin
     n:=StrToInt(Edit1.Text);
     Edit1.text:=FromDec(n,16);
    end
  else if SS1=2 then
    begin
     k:=0;
     s:=Edit1.Text;
     n:=Length(s);
     for m:=1 to n do begin
       k:=k*2;
       case s[m] of
         '0': k:=k+0;
         '1': k:=k+1;
       end;
     end;
     Edit1.Text:=IntToStr(k);
     n:=StrToInt(Edit1.Text);
   Edit1.text:=FromDec(n,16);
   end
  else if SS1=8 then
    begin
   k:=0;
   s:=Edit1.Text;
   n:=Length(s);
   for m:=1 to n do begin
     k:=k*8;
     case s[m] of
       '0': k:=k+0;
       '1': k:=k+1;
       '2': k:=k+2;
       '3': k:=k+3;
       '4': k:=k+4;
       '5': k:=k+5;
       '6': k:=k+6;
       '7': k:=k+7;
     end;
   end;
   Edit1.Text:=IntToStr(k);
   n:=StrToInt(Edit1.Text);
   Edit1.text:=FromDec(n,16);
 end;

   SS1:=16;
   Edit2.Text:=inttostr(SS1);
  Button1.Enabled:=true;
  Button2.Enabled:=true;
  Button3.Enabled:=true;
  Button4.Enabled:=true;
  Button5.Enabled:=true;
  Button6.Enabled:=true;
  Button7.Enabled:=true;
  Button8.Enabled:=true;
  Button9.Enabled:=true;
  Button0.Enabled:=true;
  Button10.Enabled:=true;
  Button11.Enabled:=true;
  Button12.Enabled:=true;
  Button13.Enabled:=true;
  Button14.Enabled:=true;
  Button15.Enabled:=true;
  end;

procedure TForm2.RadioButton3Change(Sender: TObject);
var s: string;
    n,m,k: integer;
begin
 if SS1=10 then
   begin
    n:=StrToInt(Edit1.Text);
    Edit1.text:=FromDec(n,8);
   end
 else if SS1=2 then
   begin
    k:=0;
    s:=Edit1.Text;
    n:=Length(s);
    for m:=1 to n do begin
      k:=k*2;
      case s[m] of
        '0': k:=k+0;
        '1': k:=k+1;
      end;
    end;
    Edit1.Text:=IntToStr(k);
    n:=StrToInt(Edit1.Text);
  Edit1.text:=FromDec(n,8);
  end
 else if SS1=16 then
   begin
  k:=0;
  s:=Edit1.Text;
  n:=Length(s);
  for m:=1 to n do begin
    k:=k*16;
    case s[m] of
      '0': k:=k+0;
      '1': k:=k+1;
      '2': k:=k+2;
      '3': k:=k+3;
      '4': k:=k+4;
      '5': k:=k+5;
      '6': k:=k+6;
      '7': k:=k+7;
      '8': k:=k+8;
      '9': k:=k+9;
      'A': k:=k+10;
      'B': k:=k+11;
      'C': k:=k+12;
      'D': k:=k+13;
      'E': k:=k+14;
      'F': k:=k+15;
    end;
  end;
  Edit1.Text:=IntToStr(k);
  n:=StrToInt(Edit1.Text);
  Edit1.text:=FromDec(n,8);
end;

  SS1:=8;
  Edit2.Text:=inttostr(SS1);
  Button1.Enabled:=true;
  Button2.Enabled:=true;
  Button3.Enabled:=true;
  Button4.Enabled:=true;
  Button5.Enabled:=true;
  Button6.Enabled:=true;
  Button7.Enabled:=true;
  Button8.Enabled:=false;
  Button9.Enabled:=false;
  Button0.Enabled:=true;
  Button10.Enabled:=false;
  Button11.Enabled:=false;
  Button12.Enabled:=false;
  Button13.Enabled:=false;
  Button14.Enabled:=false;
  Button15.Enabled:=false;

end;

procedure TForm2.RadioButton4Change(Sender: TObject);
var s: string;
    n,m,k: integer;
begin
 if SS1=10 then
   begin
    n:=StrToInt(Edit1.Text);
    Edit1.text:=FromDec(n,2);
   end
 else if SS1=8 then
   begin
    k:=0;
    s:=Edit1.Text;
    n:=Length(s);
    for m:=1 to n do begin
      k:=k*8;
      case s[m] of
        '0': k:=k+0;
        '1': k:=k+1;
        '2': k:=k+2;
        '3': k:=k+3;
        '4': k:=k+4;
        '5': k:=k+5;
        '6': k:=k+6;
        '7': k:=k+7;
      end;
    end;
    Edit1.Text:=IntToStr(k);
    n:=StrToInt(Edit1.Text);
  Edit1.text:=FromDec(n,2);
  end
 else if SS1=16 then
   begin
  k:=0;
  s:=Edit1.Text;
  n:=Length(s);
  for m:=1 to n do begin
    k:=k*16;
    case s[m] of
      '0': k:=k+0;
      '1': k:=k+1;
      '2': k:=k+2;
      '3': k:=k+3;
      '4': k:=k+4;
      '5': k:=k+5;
      '6': k:=k+6;
      '7': k:=k+7;
      '8': k:=k+8;
      '9': k:=k+9;
      'A': k:=k+10;
      'B': k:=k+11;
      'C': k:=k+12;
      'D': k:=k+13;
      'E': k:=k+14;
      'F': k:=k+15;
    end;
  end;
  Edit1.Text:=IntToStr(k);
  n:=StrToInt(Edit1.Text);
  Edit1.text:=FromDec(n,2);
end;

  SS1:=2;
  Edit2.Text:=inttostr(SS1);
  Button1.Enabled:=true;
  Button2.Enabled:=false;
  Button3.Enabled:=false;
  Button4.Enabled:=false;
  Button5.Enabled:=false;
  Button6.Enabled:=false;
  Button7.Enabled:=false;
  Button8.Enabled:=false;
  Button9.Enabled:=false;
  Button0.Enabled:=true;
  Button10.Enabled:=false;
  Button11.Enabled:=false;
  Button12.Enabled:=false;
  Button13.Enabled:=false;
  Button14.Enabled:=false;
  Button15.Enabled:=false;
end;


end.

