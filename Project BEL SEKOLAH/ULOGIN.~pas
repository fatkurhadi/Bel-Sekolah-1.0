unit ULOGIN;

interface

uses
  Windows, Messages, SysUtils, Variants, Classes, Graphics, Controls, Forms,
  Dialogs, StdCtrls, Buttons, DB, ADODB, jpeg, ExtCtrls;

type
  TFLOGIN = class(TForm)
    Label1: TLabel;
    Edit1: TEdit;
    ADO1: TADOConnection;
    BitBtn1: TBitBtn;
    Image1: TImage;
    procedure BitBtn1Click(Sender: TObject);
  private
    { Private declarations }
  public
    { Public declarations }
  end;

var
  FLOGIN: TFLOGIN;

implementation

uses UnitBELSEKOLAH;

{$R *.dfm}

procedure TFLOGIN.BitBtn1Click(Sender: TObject);
begin
  ADO1.ConnectionString := 'Provider=SQLOLEDB.1;Integrated Security=SSPI;Persist Security Info=False;Initial Catalog=BEL_SEKOLAH;Data Source='+EDIT1.TEXT;
  ADO1.Connected := True;
  BitBtn1.Enabled := False;
  form_Bel_Sekolah.Timer1.Enabled := True;
  Close;
end;

end.
