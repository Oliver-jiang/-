# coding: utf-8
import pickle
import argparse

def obtain_args():
    parser = argparse.ArgumentParser(description="Read pickle")
    parser.add_argument('--filename', type=str, default=None,help='file name')
    args = parser.parse_args()
    return args
    
def main():
    args=obtain_args()
    with open("D:\web download\pdb\jyc.pkl", 'rb') as f:
        f.seek(0)
        data = pickle.load(f,encoding='iso-8859-1')   #python3一定要加上encoding代码
        #data = pickle.load(f)
        print(data['atomDistMatrix']['CbCb'])
        #for labels
        print('keys:',data.keys())
        print('ACC:',data['ACC'].shape)
        print('atomDistMatrix:',data['atomDistMatrix']['CbCb'].shape)
        print(type(data['atomDistMatrix']['CbCb']))
        print(data['atomDistMatrix']['CbCb'].dtype)
         
        #for data    
#        print('keys:',data.keys())
#        print('ACC:',data['ACC'].shape)
#        #print(data[1]['ACC'].shape)
#        print('PSFM:',data['PSFM'].shape)
#        print('PSSM:',data['PSSM'].shape)
#        print('ccmpredZ:',data['ccmpredZ'].shape)
#        print('ccmpred:',data['ccmpred'].shape)
#        print('SS3:',data['SS3'].shape)
#        print('SS8:',data['SS8'].shape)
#        print('DISO:',data['DISO'].shape)
#        print('OtherPairs',data['OtherPairs'].shape)
#        f.close()
        
        #print(X.shape)

        #plt.savefig("/mnt/groupproflizhen/jiangyuncheng/1a0b_label.png") 
        #np.savetxt("/mnt/groupproflizhen/jiangyuncheng/dist.txt",np.array(data['atomDistMatrix']['CbCb']))

if __name__ == "__main__":
   main()
