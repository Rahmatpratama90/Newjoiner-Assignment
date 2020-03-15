#include <iostream>

using namespace std;

int main(){

int perintah = 1;
string nama;
string list[1000];
int uang[100];
int nomorakun;
int deposito;
int tarik;
int trf;
int nomorakun1;
int jumlah = 0;

while (perintah != 6){
	cout << "1.Daftar" << endl << 	"2.Cek Saldo" << endl << "3.Setor" 		<< endl << "4.Tarik" << endl << "5.Transfer" << endl << "6.Quit" 		<< endl << "Masukan perintah "; 
		
	cin >> perintah;
	cout << endl;
	
	if(perintah == 1){
		cout << "Masukan nama :" << endl;
		cin >> nama;
		for(int p = 0;p-1<jumlah;++p){
			if(nama==list[p]){
				cout << "Nama telah terdaftar" << endl << endl;
				break;
			}
			else{
				list[jumlah] = nama;
				cout << nama << " berhasil terdaftar" << endl << endl;
				jumlah +=1;
				break;
			}				
		}

	}
	else if(perintah == 2){
		if(jumlah!=0){
			for(int i=0;i<jumlah;++i){
			cout << i+1 << "." << list[i] << endl;
			}
			cout << "Pilih akun:";
			cin >> nomorakun;
			if(nomorakun>jumlah){
				cout << "Tolong masukan perintah yang benar" << endl 					<< endl;	
				return 0;
			}
			else if(nomorakun <=jumlah){
				cout << "Saldo:" << uang[nomorakun - 1] << endl << 					endl;
			}
		}	
		else{
			cout << "Belum ada akun yang terdaftar" << endl << endl;
		}
		
	}
	else if(perintah == 3){
		if(jumlah!=0){
			for(int i=0;i<jumlah;++i){
			cout << i+1 << "." << list[i] << endl;
			}
			cout << "Pilih akun:";
			cin >> nomorakun;
			if(nomorakun>jumlah){
				cout << "Tolong masukan perintah yang benar" << endl 					<<	endl;	
				return 0;
			}
			else if(nomorakun<=jumlah){
				cout << "Masukan jumlah uang:";
				cin >> deposito;
				cout << "Setoran berhasil" << endl << endl;
				uang[nomorakun-1] += deposito ;
			}
		}
		else{
			cout << "Belum ada akun terdaftar" << endl << endl;
		}
	}
	else if(perintah == 4){
		if(jumlah!=0){
			for(int i=0;i<jumlah;++i){
			cout << i+1 << "." << list[i] << endl;
			}
			cout << "Pilih akun:";
			cin >> nomorakun;
			if(nomorakun>jumlah){
				cout << " Masukkkan perintah yang benar" << endl 					<<	endl;	
				return 0;
			}
			else if(nomorakun<=jumlah){
				cout << "Masukan jumlah uang:";
				cin >> tarik;
				if(tarik>uang[nomorakun-1]){
					cout << "Saldo tidak mencukupi" << endl << 						endl;	
				}
				else{
					cout << "Penarikan berhasil" << endl;
					uang[nomorakun-1] -= tarik;
					cout << "Sisah saldo:" << uang[nomorakun-1] << 						endl << endl;
				}
			}
		}
		else{
			cout << "Belum ada akun yang terdaftar" << endl << endl;
		}
	}
	else if(perintah == 5){
		if(jumlah!=0){
			for(int i=0;i<jumlah;++i){
			cout << i+1 << "." << list[i] << endl;
			}
			cout << "Pilih akun:";
			cin >> nomorakun;
			if(nomorakun>jumlah){
				cout << "Masukkan perintah yang benar" << endl 					<<	endl;	
				return 0;
			}
			else if(nomorakun<=jumlah){
				cout << "Masukkan jumlah uang yang ingin di transfer:";
				cin >> trf;
				if(trf>uang[nomorakun-1]){
				cout << "Saldo tidak mencukupi" << endl << endl;	
				}
				else{
					for(int i=0;i<jumlah;++i){
					cout << i+1 << "." << list[i] << endl;
					}
				
					cout << "Pilih akun untuk ditransfer:" << endl;
					cin >> nomorakun1;
					uang[nomorakun1-1] += trf;
					uang[nomorakun-1] -= trf;
					cout << "Transfer berhasil" << endl << endl;
				}
			}	
			
		else{
			cout << "Belum ada akun yang terdaftar" << endl << endl;
		}
	}
	else if(perintah == 6){
		cout << "Terimakasih" << endl;
		return 0;	
	}
	else{
		cout << "Masukkan perintah yang benar" << endl << 		endl;	
		return 0;
	}
}
